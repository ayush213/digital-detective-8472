# Mission 7 — How computers communicate

## 1. Mission title
Mission 7: Computer networks

## 2. Task / objective
Explain basic network types and concepts, observe connectivity and DNS information, and describe what happens when a website opens.

## 3. Work completed

### Task 7.1 — Network concepts

| Concept | Explain it in your own words | Example |
|---|---|---|
| LAN | A network that covers a small area where devices are close together | Wi-Fi at home or a computer lab |
| MAN | A network that covers a whole city or a large campus | A college campus network |
| WAN | A network that covers a very large area, even across countries | The internet |
| DNS | A system that changes a website name into its IP address | Turning example.com into a number address |
| Router | A device that connects networks and sends data to the right place | My home Wi-Fi router |
| Protocol | A set of rules that devices follow so they can understand each other | HTTP and HTTPS for websites |
| Packet switching | Data is cut into small packets that travel separately and are joined again at the end | Loading a web page |
| Client-server | The client asks for something and the server sends it back | My browser asking a website's server for a page |

### Task 7.2 — Observing network information

I ran `ping -c 4 example.com` and `nslookup example.com`.

- **Ping result:** 4 packets were sent and 4 were received with 0% packet loss. The average reply time was about 14.8 ms, so example.com was reachable.
- **DNS lookup result:** `nslookup` showed the public IP addresses 172.66.147.243 and 104.20.23.154 for example.com. The lookup was answered by a public DNS server.

Answers:
- **What a connectivity test helps check:** it shows whether my computer can reach another computer or website, and how long the reply takes.
- **What a DNS lookup displays:** it shows the IP address that belongs to a domain name.
- **Role of DNS when I type a website name:** the browser asks DNS for the IP address of that name, because computers connect using IP addresses and not names.

### Task 7.3 — What happens when I open a website

1. I type a website address in the browser. The browser is the client.
2. The browser asks DNS for the IP address of that website name.
3. DNS replies with the IP address.
4. The browser sends a request, using a protocol like HTTPS, through my router and across the internet to the server with that IP address.
5. The data travels as small packets, and the router sends them along the right path.
6. The server receives the request and sends the web page back as a response.
7. The packets arrive at my computer, are joined together and the browser shows the page on my screen.

## 4. Commands / tools used
- `ping -c 4 example.com` : checks if my computer can reach the website and shows the reply time
- `nslookup example.com` : shows the IP address linked to the domain name
- VS Code (editor and Terminal) and Git (add, commit, push)

I did not publish my own IP address, Wi-Fi name or other private network details.

## 5. My understanding
A network connects devices so they can share data. LAN, MAN and WAN are different in how big an area they cover. When I open a website, DNS finds the IP address, my browser as the client sends a request using a protocol, and the server sends back the page in packets. A connectivity test like ping tells me if the other computer can be reached.

## 6. Difficulties faced
No major difficulties.

## 7. How I resolved them
Not applicable.

## 8. Evidence / files
- `mission-07-networking/README.md`

## 9. Commit details
Commit message: "Explain networking concepts and website communication". The work was pushed to GitHub and verified.