1. Initialize Git in Your Project

- Navigate to your project directory in the terminal and run:

```bash
git init
```

2. Configure Username & Email

- Check your Git username and email:

```bash
git config user.name
git config user.email
```

- If they are not set, you can set them using:

```bash
git config --global user.name "<your_github_username>"
git config --global user.email "<your_github_email>"
```

3. Check Project Status

To see the status of your project (which files are tracked, untracked, or staged):

```bash

git status
```

4. Add Files to Staging Area

- To add specific files to the staging area:

```bash
git add <file_or_folder_path>
```

- To add all files:

```bash
git add .
```

5. Commit Changes

Commit the staged files with a message:

```bash
git commit -m "your commit message"
```

6. Amend Last Commit

If you want to modify the message of your last commit:

```bash
git commit --amend
```

7. View Commit Logs

To see the commit history in a simple one-line format:

```bash
git log --oneline
```

8. Add Remote Repository

Connect your local repository to a remote GitHub repository:

```bash
git remote add origin <repository_url>
```

9. Check Branch Name

To check the current branch name:

```bash
git branch
```

10. Rename Branch

If you want to rename your current branch:

```bash
git branch -M <new_branch_name>
```

11. Push Changes to Remote

Push your changes to a remote branch:

```bash

git push origin <branch_name>
```

12. Create and Switch to a New Branch

To create and switch to a new branch:

```bash
git checkout -b <branch_name>
```

13. Switch to an Existing Branch

To switch to an existing branch:

```bash
git checkout <branch_name>
```

14. Pull Latest Changes

Pull the latest changes from the remote branch:

```bash
git pull origin <branch_name>
```

15. Add Multiple Files

To add all modified files at once:

```bash
git add .
```

16. To Clone others Repository Codes

```bash
git clone <github-repo-link>
```




