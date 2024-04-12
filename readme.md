# Tech 258 - Git

## What is version control?
Version control is the practice of tracking and managing changes to software code. Version Control Systems (VCS) are software tools that help teams manage changes to source code over time, e.g Git.

## What is git, how does it work?
Git is a open-source distributed VCS that helps developers track changes to their codebase. Git works mainly with the idea of 3 states being Modified files, Staged files and Committed files:

- Modified files: The file has been changed but has not been committed to the database yet.
- Staged files: The modified file has been marked in its current version to go into your next commit snapshot.
- Committed files: The data is safely stored in your local database.

## Showcase the basic git command flow.
### `git init`
This command creates an empty Git repository or reinitialise an existing one.
### `git status`
This command displays the current state of the repository. It shows which files have been modified, staged for commit and untracked files.
### `git add`
This command adds modified or new files to the staging area, preparing them to be included in the next commit.
### `git commit`
This command creates a new commit containing the changes that have been staged previously. Also, developers are prompted to provide a commit message describing the changes made in the commit.

## Useful extra commands
### `git log`
This command displays the commit history of the repository, showing commits in a reverse chronological order. It also provides information such as commit author, message and date.
### `git diff`
This command is used to display the differences between changes made to files in the working directory and the staging area or between commits.

## What is .gitignore and why should we use it?
A .gitignore file is used to specify intentionally untracked files that Git should ignore. It is good in the case of preventing sensitive information, artifact builds and temporary files being tracked and committed.

