# Mission 5 — Numbers and data

## 1. Mission title
Mission 5: Number systems, Python and text encoding

## 2. Task / objective
Convert numbers between decimal, binary and hexadecimal, check the results with Python, build a small number converter and explain how text is stored.

## 3. Work completed

### Task 5.1 — Conversions by hand

| Question | Working | Answer |
|---|---|---|
| Decimal 13 to binary | 13 ÷ 2 = 6 remainder 1, 6 ÷ 2 = 3 remainder 0, 3 ÷ 2 = 1 remainder 1, 1 ÷ 2 = 0 remainder 1. Reading the remainders from bottom to top gives 1101 | 1101 |
| Decimal 25 to binary | 25 ÷ 2 = 12 remainder 1, 12 ÷ 2 = 6 remainder 0, 6 ÷ 2 = 3 remainder 0, 3 ÷ 2 = 1 remainder 1, 1 ÷ 2 = 0 remainder 1. Bottom to top gives 11001 | 11001 |
| Binary 1010 to decimal | 1×8 + 0×4 + 1×2 + 0×1 = 8 + 2 | 10 |
| Binary 1101 to decimal | 1×8 + 1×4 + 0×2 + 1×1 = 8 + 4 + 1 | 13 |
| Hexadecimal A to decimal | A stands for 10 | 10 |
| Hexadecimal 1F to decimal | 1×16 + F×1 = 16 + 15 | 31 |
| Binary 1111 to hexadecimal | 1111 = 8 + 4 + 2 + 1 = 15, and 15 is F in hexadecimal | F |

### Task 5.2 — Verification using Python

I opened the Python interactive mode with `python3` and tested each conversion.

| Expression | Result | Matches my manual answer? |
|---|---|---|
| `bin(13)` | `'0b1101'` | Yes (1101) |
| `bin(25)` | `'0b11001'` | Yes (11001) |
| `int("1010", 2)` | `10` | Yes |
| `int("1101", 2)` | `13` | Yes |
| `hex(10)` | `'0xa'` | Yes (A) |
| `hex(31)` | `'0x1f'` | Yes (1F) |
| `int("A", 16)` | `10` | Yes |
| `int("1F", 16)` | `31` | Yes |
| `hex(15)` | `'0xf'` | Yes (F) |

The `0b` at the start of a result means the number is in binary, and `0x` means it is in hexadecimal.

### Task 5.3 — Number converter

The file `number_converter.py` asks the user for a decimal number and shows it in binary and hexadecimal. I ran it with `python3 number_converter.py` and tested three numbers.

| Test number | Binary output | Hexadecimal output |
|---|---|---|
| 10 | 0b1010 | 0xa |
| 25 | 0b11001 | 0x19 |
| 255 | 0b11111111 | 0xff |

How the program works:
- `input()` takes what the user types as text.
- `int()` changes that text into a whole number.
- `bin()` gives the binary form of the number as text.
- `hex()` gives the hexadecimal form of the number as text.
- `print()` shows the results.

### Task 5.4 — How is text stored?

- **ASCII codes:** uppercase A is 65 and lowercase a is 97. I checked them with `ord("A")` and `ord("a")` in Python.
- **Why an encoding standard is needed:** a computer can only store numbers, so every character has to be given a fixed number. Without a common standard, different computers would show the same stored data as different text.
- **A character not in basic ASCII:** the rupee sign ₹ (also é or an emoji).

## 4. Commands / tools used
- `python3` : opened Python interactive mode to test conversions
- `bin()` : converts a number to binary text
- `hex()` : converts a number to hexadecimal text
- `int(text, base)` : converts binary or hexadecimal text to a decimal number
- `input()` : reads what the user types
- `print()` : displays results
- `ord()` : shows the ASCII code of a character
- `python3 number_converter.py` : ran the converter program
- VS Code (editor and Terminal) and Git (add, commit, push)

## 5. My understanding
Computers store everything as bits, which are 0 or 1, and eight bits make a byte. Binary uses base 2, decimal uses base 10 and hexadecimal uses base 16, so the same number can be written in different ways. I did the conversions by hand and then checked them with Python's `bin()`, `hex()` and `int()` functions, and all the results matched. For text, a computer uses an encoding like ASCII or UTF-8 to turn each character into a number.

## 6. Difficulties faced
I typed `pyhton3` by mistake and got "command not found". I also pasted the Python lines into the Terminal before Python was open, so they did not run.

## 7. How I resolved them
I corrected the spelling to `python3`. I then waited for the `>>>` prompt to appear before typing the Python expressions.

## 8. Evidence / files
- `mission-05-numbers-data/README.md`
- `mission-05-numbers-data/number_converter.py`

## 9. Commit details
Commit message: "Build number converter and practise data representation". The work was pushed to GitHub and verified.