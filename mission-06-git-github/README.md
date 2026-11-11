# Mission 6 — Git and GitHub

## 1. Mission title
Mission 6: Git, GitHub, branches and Pull Requests

## 2. Task / objective
Understand version control, stage and commit changes, create a branch, open a Pull Request and explain the collaboration workflow.

## 3. Work completed

### Task 6.1 — Basic Git workflow
I checked the repository status, staged the root README, committed it with a meaningful message and looked at the commit history.

| Git operation | What it does in your own words |
|---|---|
| Check repository status (`git status`) | Shows which files are changed, staged or untracked |
| Stage selected changes (`git add README.md`) | Puts the chosen file in the staging area, which is the list of changes that will go into the next commit |
| Create a commit (`git commit -m "..."`) | Saves a snapshot of the staged changes in the history with a message |
| View commit history (`git log --oneline`) | Shows the earlier commits, newest first |

**Staging vs committing:** staging chooses which changes will be saved, and committing actually saves them as a snapshot in the history.

### Task 6.2 — Branch
I created a branch named `update-about` with `git checkout -b update-about`. In the root README I added a "My Learning" section with three things I learned. I checked the status, staged the README, committed it ("Add My Learning section to README") and pushed the branch to GitHub with `git push -u origin update-about`.

### Task 6.3 — Pull Request
I opened a Pull Request on GitHub from `update-about` into `main` with a short description of the README change.

**PR status:** The Pull Request is open and not merged.

- **Branch:** a separate line of work in a repository. I can try changes on it without touching the main branch.
- **Pull Request:** a request on GitHub to bring the changes of one branch into another, like `update-about` into `main`. Other people can look at the changes before they are merged.
- **Why they are useful:** when many people work on one project, branches keep everyone's work separate, and Pull Requests let the team review changes first, so mistakes and conflicts are caught early.

### Task 6.4 — Git command glossary

| Git operation | One-line explanation |
|---|---|
| Initialise a repository (`git init`) | Starts Git tracking in a folder |
| Check status (`git status`) | Shows changed, staged and untracked files |
| Stage changes (`git add`) | Selects changes for the next commit |
| Commit changes (`git commit`) | Saves the staged changes as a snapshot with a message |
| View history (`git log`) | Lists the earlier commits |
| Create or list branches (`git branch`, `git checkout -b`) | Lists branches or makes a new one |
| Switch branches (`git switch`) | Moves to a different branch |
| Publish changes (`git push`) | Uploads my commits to GitHub |
| Retrieve remote changes (`git pull`) | Brings the latest changes from GitHub to my computer |

## 4. Commands / tools used
- `git status` : checks the state of my files
- `git add` : stages changes
- `git commit -m` : saves a snapshot
- `git log --oneline` : shows the history
- `git checkout -b` and `git switch` : create and move between branches
- `git branch` : lists branches
- `git push -u origin update-about` : publishes the new branch
- GitHub website : used for the Pull Request
- VS Code (editor and Terminal)

## 5. My understanding
Git saves the history of my files so I can go back and work safely. Staging chooses what goes into the next commit and committing saves it. A branch lets me work on a change separately from `main`, and a Pull Request is how that change is shown on GitHub before it joins `main`. The "My Learning" section appears only on the `update-about` branch until the Pull Request is merged.

## 6. Difficulties faced
My first commit on `update-about` showed "nothing to commit" because the new text had not been saved in the README yet. The Pull Request banner also did not appear on GitHub.

## 7. How I resolved them
I saved the file and checked `git status` before committing, and used the Branches page and the compare page on GitHub to find the branch.

## 8. Evidence / files
- `mission-06-git-github/README.md`
- Branch `update-about` on GitHub
- Root `README.md` (My Learning section on the `update-about` branch)

## 9. Commit details
Commit message: "Complete Git and GitHub collaboration mission". The work was pushed to GitHub and verified.