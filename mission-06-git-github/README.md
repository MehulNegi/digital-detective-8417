# Mission 6 — Git and GitHub

## 1. Task / objective

Practise staging and committing changes, publishing a branch and opening a pull request. Explain how these steps help people collaborate on the same repository.

## 2. Work completed

I checked the repository status and created a branch called `update-about`. On that branch, I added a **My Learning** section to the root README. I staged the README, committed the change and checked the recent commit history.

I pushed `update-about` to GitHub and opened a pull request into `main`. I reviewed the **Files changed** tab and checked that it showed only the root README change. The pull request is open on GitHub.

## 3. Commands / tools used

| Git operation | Command | What it does |
|---|---|---|
| Initialise a repository | `git init` | Sets up Git tracking in the current directory. |
| Check status | `git status` | Shows the current branch and which files are staged, modified or untracked. |
| Stage selected changes | `git add README.md` | Selects the current changes to the root README for the next commit. |
| Review staged files | `git diff --cached --name-only` | Lists the files selected for the next commit. |
| Create a commit | `git commit -m "Add learning summary to the root README"` | Saves the staged changes in the branch's history with a message. |
| View history | `git log -3 --oneline` | Shows the three most recent commits in a compact format. |
| Create or list branches | `git switch -c update-about` or `git branch` | Creates and switches to a new branch, or lists local branches. |
| Switch branches | `git switch main` | Switches the working directory back to `main`. |
| Publish changes | `git push -u origin update-about` | Publishes the branch on GitHub and sets its upstream branch. |
| Retrieve remote changes | `git pull --ff-only` | Fetches remote changes and updates the current branch if it can move forward without a merge commit. |

I used GitHub to open the pull request and review the changed file.

## 4. My understanding

Staging puts selected changes into the next commit. Committing saves those staged changes in the branch's history. I staged only the root README for the learning update so I could check exactly what would go into that commit.

A branch gives me a place to work on a change independently of `main`. A pull request shows what would change if the branch were merged. It gives collaborators a place to review the changes and discuss them before they go into the shared branch.

## 5. Difficulties faced

No major difficulties.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

- The root `README.md` on `update-about` contains the **My Learning** section.
- The repository's **Pull requests** tab shows the PR titled `Add My Learning section to the root README`.
- This README contains the Git command glossary and my explanation of the workflow.

## 8. Commit details

- Branch commit — `Add learning summary to the root README`
- Mission commit — `Complete Git and GitHub collaboration mission`
- Push verification — See this file's **History** on GitHub for the published mission commit.