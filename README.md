---
# **Git Commands**
---

## **Getting Started**

| **Command**                                                                                                        | **Description**                                              |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------ |
| `git init`                                                                                                         | Initialize a local Git repository in your project directory. |
| `git config user.name`<br>`git config user.email`                                                                  | Check the configured username and email for Git.             |
| `git config --global user.name "<your_github_username>"`<br>`git config --global user.email "<your_github_email>"` | Set your Git username and email globally.                    |
| `git config --list`                                                                                                | View all Git configurations.                                 |
| `git help <command>`                                                                                               | Get help for a specific Git command.                         |
| `git version`                                                                                                      | Check your installed Git version.                            |

---

## **Basic Snapshotting**

| **Command**                           | **Description**                                                         |
| ------------------------------------- | ----------------------------------------------------------------------- |
| `git status`                          | Show the current state of the working directory and staging area.       |
| `git add <file_or_folder_path>`       | Add specific files or folders to the staging area.                      |
| `git add .`                           | Add all changes (new, modified, and deleted files) to the staging area. |
| `git commit -m "your commit message"` | Commit staged changes with a descriptive message.                       |
| `git commit --amend`                  | Modify the last commit (message or staged changes).                     |
| `git restore <file_name>`             | Discard changes to a specific file (unstaged changes).                  |
| `git restore --staged <file_name>`    | Remove a file from the staging area without deleting it.                |

---

## **Viewing History**

| **Command**                 | **Description**                             |
| --------------------------- | ------------------------------------------- |
| `git log`                   | View a detailed history of commits.         |
| `git log --oneline`         | View a condensed commit history.            |
| `git log --graph --oneline` | Visualize branch history in a graph format. |
| `git show <commit_hash>`    | Show details of a specific commit.          |

---

## **Branching & Working with Branches**

| **Command**                       | **Description**                                                                          |
| --------------------------------- | ---------------------------------------------------------------------------------------- |
| `git branch`                      | Display a list of branches (current branch is marked with an asterisk).                  |
| `git branch -a`                   | List all branches (local and remote).                                                    |
| `git branch <branch_name>`        | Create a new branch.                                                                     |
| `git branch -d <branch_name>`     | Delete a branch.                                                                         |
| `git branch -M <new_branch_name>` | Rename the current branch.                                                               |
| `git checkout -b <branch_name>`   | Create a new branch and switch to it.                                                    |
| `git checkout <branch_name>`      | Switch to an existing branch.                                                            |
| `git checkout -`                  | Switch back to the previous branch.                                                      |
| `git merge --no-ff <branch_name>` | Merge a branch into the current branch without fast-forwarding (creates a merge commit). |

---

## **Stashing Changes**

| **Command**       | **Description**                                                                         |
| ----------------- | --------------------------------------------------------------------------------------- |
| `git stash`       | Temporarily save changes in a dirty working directory.                                  |
| `git stash pop`   | Apply the most recent stash to the working directory and remove it from the stash list. |
| `git stash list`  | View all stashed entries.                                                               |
| `git stash apply` | Apply a specific stash without removing it from the stash list.                         |
| `git stash drop`  | Remove a specific stash.                                                                |
| `git stash clear` | Remove all stashed entries.                                                             |

---

## **Remote Repositories**

| **Command**                                      | **Description**                                                     |
| ------------------------------------------------ | ------------------------------------------------------------------- |
| `git remote add origin <repository_url>`         | Link a local repository to a remote repository.                     |
| `git remote -v`                                  | View the configured remote repositories.                            |
| `git remote set-url origin <new_repository_url>` | Change the URL of the remote repository.                            |
| `git fetch`                                      | Download objects and refs from a remote repository without merging. |
| `git clone <repository_url>`                     | Create a local copy of a remote repository.                         |

---

## **Pushing Changes**

| **Command**                        | **Description**                                                          |
| ---------------------------------- | ------------------------------------------------------------------------ |
| `git push origin <branch_name>`    | Push changes to a specific branch on the remote repository.              |
| `git push -u origin <branch_name>` | Push changes and set the remote branch as the default for future pushes. |
| `git push`                         | Push changes to the remote branch (default branch).                      |
| `git push --force`                 | Force push changes to overwrite remote changes (use with caution).       |

---

## **Pulling Changes**

| **Command**                     | **Description**                                                              |
| ------------------------------- | ---------------------------------------------------------------------------- |
| `git pull origin <branch_name>` | Fetch and merge changes from a remote branch.                                |
| `git pull`                      | Update the local branch with the latest changes from its remote counterpart. |
| `git pull --rebase`             | Rebase the current branch on top of the fetched branch.                      |

---

## **Merging Changes**

| **Command**                                 | **Description**                                        |
| ------------------------------------------- | ------------------------------------------------------ |
| `git merge <branch_name>`                   | Merge a specified branch into the current branch.      |
| `git merge <source_branch> <target_branch>` | Merge a source branch into a target branch.            |
| `git merge --squash <branch_name>`          | Squash all commits from a branch into a single commit. |

---

## **Undoing Changes**

| **Command**                | **Description**                                                                        |
| -------------------------- | -------------------------------------------------------------------------------------- |
| `git reset <file_name>`    | Unstage a file but keep the changes in the working directory.                          |
| `git reset --hard`         | Reset the working directory and staging area to the last commit. All changes are lost. |
| `git revert <commit_hash>` | Create a new commit that reverses changes introduced by a specific commit.             |
| `git clean -fd`            | Remove all untracked files and directories.                                            |

---

## **Inspection & Comparison**

| **Command**                                | **Description**                                 |
| ------------------------------------------ | ----------------------------------------------- |
| `git diff`                                 | Show changes not staged for commit.             |
| `git diff --staged`                        | Show changes staged for commit.                 |
| `git diff <source_branch> <target_branch>` | Compare two branches before merging.            |
| `git blame <file_name>`                    | Show who modified each line of a file and when. |

---

## **Tagging**

| **Command**                              | **Description**                               |
| ---------------------------------------- | --------------------------------------------- |
| `git tag <tag_name>`                     | Create a new tag.                             |
| `git tag -a <tag_name> -m "tag message"` | Create an annotated tag with a message.       |
| `git push origin <tag_name>`             | Push a specific tag to the remote repository. |
| `git push --tags`                        | Push all tags to the remote repository.       |
| `git tag -d <tag_name>`                  | Delete a local tag.                           |
| `git push origin --delete <tag_name>`    | Delete a remote tag.                          |

---
