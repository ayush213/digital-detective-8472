# Mission 4 — How programs run

## 1. Mission title
Mission 4: How programs run

## 2. Task / objective
Run a simple Python program and compare how compilers and interpreters translate or run programs.

## 3. Work completed

### Task 4.1 — Create and run a Python program
I created a file named `hello.py` in this folder with a one-line program that prints a message. I ran it with Python 3 from the Terminal and the message `Hello from Python` appeared.

### Task 4.2 — Compiler vs interpreter

| Point | Compiler | Interpreter |
|---|---|---|
| When translation / execution happens | The whole program is translated before it runs | The program is read and run line by line while it runs |
| Typical output | A separate executable (machine code) file | No separate file, the result appears directly |
| One example | C (using gcc) | Python |
| One advantage | The finished program runs fast, and many errors are caught before running | Easy to test, because I can run the code immediately without a build step |

A compiler translates the whole source code into machine code before the program runs, so it creates a separate file that can be run later. An interpreter reads and runs the instructions one by one while the program is running. In my table, C is an example of a compiled language and Python is an example of an interpreted language. Real languages can mix both, for example Python first turns code into bytecode and then runs it.

## 4. Commands / tools used
- `echo` : wrote the one-line program into `hello.py`
- `cat` : showed the contents of the file
- `python3 hello.py` : ran the program with Python 3
- VS Code (editor and Terminal) and Git (add, commit, push)

## 5. My understanding
Running a program means the computer follows its instructions. I ran hello.py with python3 and saw the message on the screen. A compiler translates everything first, while an interpreter runs the code step by step, so Python programs can be tested quickly.

## 6. Difficulties faced
No major difficulties.

## 7. How I resolved them
Not applicable.

## 8. Evidence / files
- `mission-04-programs/hello.py`
- `mission-04-programs/README.md`

## 9. Commit details
Commit message: "Compare compilers and interpreters". The work was pushed to GitHub and verified.