# Mission 3 — Understand the operating system

## 1. Mission title
Mission 3: Operating system, processes and permissions

## 2. Task / objective
Explore the operating system, running processes, storage, paths and file permissions, and describe the responsibilities of an operating system.

## 3. Work completed

### Task 3.1 — Explore my operating system

| Information explored | What it tells you | Your observation (privacy-safe) |
|---|---|---|
| Operating system / system details (`uname -a`) | Which OS and kernel the computer runs, and the type of processor | Darwin kernel version 27.2.0 (the core of macOS) on arm64 (Apple silicon). Device name: [redacted] |
| Current account identity (`whoami`) | Which user account is currently active | The active account is [redacted] |
| Available and used storage (`df -h`) | How much disk space is total, used and free | About 926 GB total with about 859 GB available. The main data volume had about 41 GB used |
| System activity snapshot (`top -l 1 \| head -15`) | What the computer is doing right now (processes, CPU, memory) | 942 processes in total, 2 running and 940 sleeping. CPU was about 94% idle |

### Task 3.2 — Processes

- **What is a process?** A process is a program that is currently running on the computer.
- **What does the PID column represent?** PID is the process identifier, a unique number the operating system gives to each running process.
- **Two examples from my computer:** Visual Studio Code (PID 25915), which is an application I was using, and WindowServer (PID 479), which is a background system process that draws the windows on the screen.

### Task 3.3 — Paths and permissions

I moved into `mission-02-terminal` and back with `cd`, and `pwd` showed the current location changing each time.

- **Absolute path:** the full path from the root of the computer, for example `/Users/[redacted]/Desktop/digital-detective-8472/mission-02-terminal`.
- **Relative path:** the path from where I am now, for example `mission-02-terminal/README.md` from the repository folder.

For `notes.txt`, `ls -l` showed `-rw-r--r--`. The first three letters (`rw-`) are for the owner: the owner can read and write the file but cannot execute it.

| Permission | Meaning | Example |
|---|---|---|
| r — Read | Allows a file's contents to be read | Opening a text file |
| w — Write | Allows a file to be changed | Editing a text file |
| x — Execute | Allows a file to be run; on a directory, allows access | Running a script |

### Task 3.4 — Operating system responsibilities

| OS responsibility | Your explanation | Example |
|---|---|---|
| Process management | Decides which programs run and when, and shares the CPU between them | Running VS Code and Terminal at the same time |
| Memory management | Gives each program some RAM and takes it back when the program closes | Closing a browser tab frees memory |
| Device management | Controls hardware like the keyboard, screen and storage through drivers | Showing what I type on the screen |
| File management | Organises, saves, finds and protects files and folders | Saving a file in a folder |
| User interface / shell | The way a person talks to the computer, either by clicking or by typing commands | The macOS desktop and the Terminal |
| Security and permissions | Controls who can read, change or run files and keeps the system protected | The `rw-` permissions on a file |

## 4. Commands / tools used
- `uname -a` : shows operating system and kernel details
- `whoami` : shows the current user account
- `df -h` : shows disk space in a readable form
- `top -l 1 | head -15` : takes a snapshot of system activity and shows the first lines
- `ps aux | head -10` : lists running processes with their PIDs
- `pwd` : shows the current folder path
- `cd` : moves between folders
- `ls -l` : shows a detailed listing with permissions
- VS Code (editor and Terminal) and Git (add, commit, push)

I replaced my username and device name with [redacted] so no private details are published.

## 5. My understanding
The operating system manages the hardware and gives services to the programs I run. A process is a running program, and each one has its own PID so the system can keep track of it. An absolute path starts from the root of the computer, while a relative path starts from the folder I am in. File permissions r, w and x decide who can read, change or run a file, which helps keep the system safe.

## 6. Difficulties faced
No major difficulties.

## 7. How I resolved them
Not applicable.

## 8. Evidence / files
- `mission-03-operating-system/README.md`

## 9. Commit details
Commit message: "Document operating system and file management". The work was pushed to GitHub and verified.