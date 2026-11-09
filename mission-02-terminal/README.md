# Mission 2 — Become comfortable with the Terminal

## 1. Mission title
Mission 2: Terminal and file management

## 2. Task / objective
Use the command-line interface to look at folders, create and manage practice files, understand flags and pipes, and explain package managers.

## 3. Work completed





### Task 2.1 — Basic Terminal operations

| Operation / command name | What it does | What I observed |
|---|---|---|
| Current-directory display (`pwd`) | Shows the full path of the folder I am working in | It showed the full path ending in digital-detective-8472, with my user folder as [redacted] |
| Directory listing (`ls`) | Lists the files and folders in the current location | It showed evidence, all the mission folders and README.md |
| Detailed listing (`ls -l`) | Lists files with details like permissions, owner, size and date | Each item was on its own line with permissions, size and modified date |
| Change directory (`cd ..`) | Moves to the parent folder | After running it, pwd showed the parent folder instead of the repository |
| Create directory (`mkdir practice`) | Creates a new folder | No message appeared, but the practice folder showed up in ls |
| Create empty file (`touch practice/original.txt`) | Creates a new empty file | No message appeared, but original.txt was visible inside practice |
| Copy file (`cp practice/original.txt practice/copy.txt`) | Makes a copy of a file with a new name | No message appeared, and both original.txt and copy.txt were in the folder |
| Move / rename file (`mv practice/copy.txt practice/renamed.txt`) | Renames or moves a file | copy.txt disappeared and renamed.txt appeared in its place |
| Display file contents (`cat practice/original.txt`) | Prints the contents of a file in the Terminal | Nothing was printed because the file was empty | 


### Task 2.2 — Practising file changes safely

I created a folder named `terminal-practice` and worked only inside it.

Commands used:
- `mkdir terminal-practice` created the folder
- `echo "This is line one" > notes.txt` created a file with the first line
- `echo "This is line two" >> notes.txt` added a second line without removing the first
- `cat notes.txt` showed both lines
- `cp notes.txt backup.txt` made a backup copy
- `mv backup.txt notes-backup.txt` renamed the backup

What I observed: `cat` printed both lines, and `ls` showed `notes.txt` and `notes-backup.txt`.

**Questions**
1. **Replacing vs adding text:** `>` replaces everything in the file with the new text, while `>>` adds the new text at the end and keeps the old lines.
2. **Copying vs moving:** Copying makes a second file and keeps the original. Moving shifts the file to a new place or name, so the old one is gone.
3. **What pwd shows:** It shows the full path of the folder I am currently in.
4. **Why ls is useful:** It shows what files and folders are in a location, so I can check that my commands worked.


### Task 2.3 — Flags and pipes

I ran `ls`, `ls -lah` and `ls -l | head -5`.

- `ls` showed only the names of the files and folders.
- `ls -lah` showed more: `-l` gave details like permissions, owner, size and date, `-a` showed hidden files such as `.git` and `.gitignore`, and `-h` showed sizes in a readable form like KB.
- In `ls -l | head -5`, the pipe `|` sends the output of the left command to the right command. `ls -l` produced the detailed list and `head -5` showed only its first 5 lines.


### Task 2.4 — Package managers

I ran `brew --version` and `brew list`. Homebrew is installed on my Mac, and the list showed the packages it manages. I did not install or uninstall anything.

A package manager installs, updates and removes software using simple commands. It is useful because it saves time, keeps software organised in one place and makes updates easy.





## 4. Commands / tools used
- `pwd` : shows the full path of the current folder
- `ls`, `ls -l`, `ls -lah` : list files, with details, hidden files and readable sizes
- `cd` : moves between folders
- `mkdir` : creates a folder
- `touch` : creates an empty file
- `cp` : copies a file
- `mv` : renames or moves a file
- `cat` : shows the contents of a file
- `echo` with `>` and `>>` : writes text to a file, replacing it or adding to the end
- `head` and the pipe `|` : show only the first lines of another command's output
- `brew --version` and `brew list` : check the package manager (Homebrew)
- VS Code (editor and Terminal) and Git (add, commit, push)

## 5. My understanding
Terminal lets me control the computer with typed commands instead of clicking. I learned that `>` replaces a file's content while `>>` adds to the end, and that copying keeps the original while moving does not. Flags like `-l`, `-a` and `-h` change how `ls` shows its output, and a pipe passes the output of one command into another. A package manager installs, updates and removes software in an organised way.

## 6. Difficulties faced
No major difficulties.

## 7. How I resolved them
Not applicable.

## 8. Evidence / files
- `mission-02-terminal/README.md`
- `mission-02-terminal/terminal-practice/notes.txt`
- `mission-02-terminal/terminal-practice/notes-backup.txt`

## 9. Commit details
Commit message: "Complete Terminal and file management mission". The work was pushed to GitHub and verified.