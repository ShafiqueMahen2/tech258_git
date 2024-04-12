# Tech 258 - Git

## What is version control?
Version control is the practice of tracking and managing changes to software code. Version Control Systems (VCS) are software tools that help teams manage changes to source code over time, e.g Git.

## What is git, how does it work?
Git is a open-source VCS that helps developers track changes to their codebase. Git works mainly with the idea of 3 states being Modified files, Staged files and Committed files:

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

## Distributed Version Control

![Alt text](/images/centralised_vs_distributed.png "Centralised VCS vs Distributed VCS diagram")

As shown by the diagram above, the Centralised VCS has a central repository that stores all versions of the files. The user's will commit to that repo and pull updates from that repo only.
The Distributed VCS on the other hand equips each user with their own local repository. This allows for the users to commit changes to their local repository and perform version control actions independently, preventing conflicts which may occur if they were to commit simultaneously to the main repo (like in the Centralised VCS example).

## What is GitHub?
GitHub facilitates remote collaboration among developers by utilising Git for hosting repositories on the web.
Essentially, it makes it a lot easier for individuals and teams to use Git for version control and collaboration.

## What are some other options/competitors?
There are many alternatives to GitHub including:

- **GitLab**: Similar to GitHub, GitLab offers a web-based Git repository manager with features for version control.
- **Bitbucket**: Similar to GitHub, BitBucket is a Git-based version control platform but owned by Atlassian. It offers integration with other Atlassian tools like Jira.
- **AWS CodeCommit**: AWS CodeCommit is a fully managed Git-based source control service provided by the cloud provider, AWS. It offers seamless integration with other AWS services.

## How do you link a local repo to a remote repo on GitHub?
To link a local Git repository to a remove repository on GitHub, you must log on to GitHub and create a new repo.
Once this is complete, execute the commands below (these are given as instructions on GitHub itself.)
```commandline
git remove add origin <enter GitHub repo link here (.git on the end!)>
git branch -M main
git push -u origin main
```
These commands will push all of the stored commits published locally to your new GitHub repo. The history of the local commits will also be published.

### How do you link a remote repo to a new local repo?
To link a remote repo to a new local repo, you must log on to GitHub and create a new repo or access an already existing repo on GitHub.
Once ready, you must execute the commands below (these are also given as instructions on GitHub, similar to the previous section.)
```commandline
echo "# tech258_git" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin <enter GitHub repo link here (.git on the end!)>
git push -u origin main
```
These commands will link the remotely created repo to your local machine!



