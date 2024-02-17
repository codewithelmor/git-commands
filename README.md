# Git Commands

Git is a distributed version control system that helps manage and track changes in source code during software development. Here are some commonly used Git commands:

1. ```Initializing a Repository```:

```git init```: Initializes a new Git repository.

2. ```Cloning a Repository```:

```git clone <repository_url>```: Creates a copy of a remote repository on your local machine.

3. ```Adding and Committing Changes```:

```git add <file>```: Adds changes in a specific file to the staging area.
```git add . or git add --all```: Adds all changes to the staging area.
```git commit -m "Commit message"```: Commits the staged changes with a descriptive message.

4. ```Checking the Status```:

```git status```: Shows the status of changes as untracked, modified, or staged.

5. ```Viewing Commit History```:

```git log```: Displays a log of all commits.

6. ```Branching```:

```git branch```: Lists all local branches.
```git branch <branch_name>```: Creates a new branch.
```git checkout <branch_name> or git switch <branch_name>```: Switches to the specified branch.
```git merge <branch_name>```: Merges changes from the specified branch into the current branch.

7. ```Remote Repositories```:

```git remote -v```: Shows a list of remote repositories.
```git remote add <name> <repository_url>```: Adds a new remote repository.
```git pull <remote> <branch>```: Fetches changes from a remote repository and merges them into the current branch.
```git push <remote> <branch>```: Pushes local changes to a remote repository.

8. ```Undoing Changes```:

```git reset <file>```: Unstages changes in a file.
```git reset --hard <commit>```: Resets the repository to a specific commit, discarding changes.
```git revert <commit>```: Creates a new commit that undoes the changes made in the specified commit.

9. ```Tagging```:

```git tag```: Lists all tags.
```git tag -a <tag_name> -m "Tag message"```: Creates an annotated tag.
```git push --tags```: Pushes tags to a remote repository.

10. ```Configuration```:

```git config --global user.name "Your Name"```: Sets your username globally.
```git config --global user.email "your@email.com"```: Sets your email globally.

These are just some of the basic Git commands. Git has a rich set of features, so it's recommended to refer to the official documentation or use ```git --help``` for more details on specific commands.

## My Common Git Commands

```bash
git init

# Clone specific branch
git clone <repository_url> -b <branch>

# Add modified files
git add -u

# Add all files
git add --all

git commit -m 'Commit message'
git push origin

# Important command when you fucked up but do not use this in a branch with CI/CD
git reset --hard <commit>
git push -f

# Remove local branches from which are untracked
git remote prune origin

# Combine multiple commits into one
git merge --squash origin/<branch>

# Checkout specific branch
git checkout <branch>

# Remove previously checked-out branch. Use this command to check-out a branch properly. Otherwise your previous commits will be pushed to the current checked-out branch
git branch -D <branch>

```
