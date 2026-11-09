# Mission 0 — Create your GitHub workspace

## 1. Mission title
Mission 0: Repository and workspace setup

## 2. Task / objective
Create a correctly named public GitHub repository and prepare the folder structure for all the missions.

## 3. Work completed
- Created the project folder `digital-detective-8472` on my computer.
- Created a separate folder and README.md for every mission (mission-00 to mission-08) and an `evidence` folder.
- Created `number_converter.py` inside the mission-05 folder.
- Wrote the root README with a mission index.
- Created a public GitHub repository with the same name and pushed the files.
- Added a `.gitignore` and removed the `.DS_Store` file that macOS had created.

## 4. Commands / tools used
- `python3 --version` : checked Python. Result: Python 3.9.6
- `git --version` : checked Git. Result: git version 2.54.0 (Apple Git-157)
- `git init` : turned the folder into a Git repository
- `git remote add origin` : linked the local folder to the GitHub repository
- `git remote -v` : checked the linked URL
- `git add` : staged files for the commit
- `git commit -m` : saved a snapshot with a message
- `git push` : uploaded commits to GitHub
- `git rm --cached` : stopped tracking `.DS_Store` without deleting my own files
- `touch` : created the `.gitkeep` file so the empty evidence folder uploads
- VS Code : text editor and terminal
- GitHub : online hosting of the repository

## 5. My understanding
A repository is a project folder tracked by Git. It stores the files and the full history of changes, so I can go back to earlier versions. The folders are organised by mission so each mission's work is kept separate and my instructor can review it one mission at a time.
Git does not track empty folders, so I added a `.gitkeep` file to `evidence`.

## 6. Difficulties faced
- Git showed "Author identity unknown" when I first tried to commit.
- My first push was rejected with "fetch first".
- A `.DS_Store` file was uploaded by mistake.

## 7. How I resolved them
- I set my name and a GitHub private email with `git config --global`.
- The GitHub repo already contained a starter commit, so I used `git push -u origin main --force` to replace it with my local version. This was safe because the repo was new.
- I added `.DS_Store` to `.gitignore` and removed it from Git with `git rm --cached`.

## 8. Evidence / files
- Root `README.md`
- `mission-00-setup/README.md`
- Folder structure of all missions on GitHub

## 9. Commit details
- Setup commit: "Set up Digital Detective mission structure", pushed to GitHub.
- Cleanup commit: "Remove .DS_Store and add .gitignore", pushed to GitHub.
- README commit: "Complete Mission 0 README", pushed to GitHub.