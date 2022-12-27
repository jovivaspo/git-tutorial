# **Git**

## **What's Git?**

"Git is a free and open source distributed version
control system designed to handle everything
from small to very large projects with speed and
efficiency”. [Source](https://git-scm.com)

## **Why should we use it?**

- Change control
- Easy to use
- Most useful with text files
- Feature management
- Teamwork
- No real server
- Remote teams
- Deployment in different environments
- Modern and evolving!

## **Installation**

- Links installation:
  - [Window](https://git-scm.com/download/win)
  - [Mac](https://git-scm.com/download/mac)
  - [Linux](https://git-scm.com/download/linux)
- Config:
  - Define Visaul Studio Code as the default editor.
  - Define the main branch as "main".

## **Basics commands**

### Configure git

- **`git config --global user.name "[name]`**: set the name you want attached to your commit.
- **`git config --global user.email "[email address]"`**: set the email you want attached to your commit.

### Set up & init:

- **`git init [project-name]`**: start a repository.
- **`git clone [url]`**: clone one repository.

### Stage & Snapshot:

- **`git init`**: start a repository.
- **`git status`**: check the repository, show modified files in working directory, staged for your next commit.
- **`git add [file]`** or **`git add .`** : add a file or git all changed files.
- **`git diff`**: diff of what is changed but not staged.
- **`git commit -m [menssage]`**: commit the change and add a descriptive message.

### Branch & Merge:

- **`git branch`**: list your branches, a \* appear next to the currently active branch.
- **`git branch [branch-name]`**: create a new branch.
- **`git checkout [branch-name]`**: select other brach.
- **`git checkout -b [branch-2] [branch-1]`**: create a branch called branch-2 from branch-1.
- **`git merge [branch]`**: merge the specified branch into the current one.
- **`git log`**: show all commits in the current branch.
- **`git log --oneline`**: show all commits in one line.

### Share & update:

- **`git remote add [url]`**: add a git url.
- **`git push [branch]`**: send local branch commits to the remote repository branch.
- **`git pull [branch]`**: fetch any commits from the remote branch.

### Tracking path changes:

- **`git rm [file]`**: delete the file from project.
- **`git mv [existing-path] [new-path]`**: change the existing file path and stage the move.

### Rewrite history:

- **`git rebase [branch]`**: apply any commits of current branch ahead of specified one.
- **`git reset --hard [commit]`**: clear staging area, rewrite working tree from specified commit.

**Others resources**:

- [Original documentation](https://git-scm.com/docs)
- [Pro Git book](https://git-scm.com/book/en/v2)
- [Git Cheat Sheets](https://training.github.com/) in different lenguages.

## **Graphical Interfaces**

- [SourceTree](https://www.sourcetreeapp.com)
- [GitKraken](https://www.gitkraken.com)

## **How to do good comments**

There 7 basic rules:

1. Separate subject from body with a blank line.
2. Limit the subject line to 50 characters.
3. Capitalize the subject line.
4. Do not end the subject line with a period.
5. Use the imperative mood in the subject line.
6. Wrap the body at 72 characters.
7. Use the body to explain what and why vs. how.

![How to write a correct commit](https://cbea.ms/content/images/size/w2000/2021/01/git_commit_2x.png)

[Source](https://chris.beams.io/posts/git-commit/)

## **Git-flow Workflow**:

Git flow is a popular Git branching strategy aimed at simplifying release management, and was introduced by software developer Vincent Driessen in 2010. Fundamentally, Git flow involves isolating your work into different types of Git branches.
In the Git flow workflow, there are five different branch types:

- Main: contains production-ready code that can be released.
- Develop: contains pre-production code with newly developed features that are in the process of being tested.
- Feature: it is used when adding new features to your code.
- Release: used when preparing new production releases
- Hotfix: used to quickly address necessary changes in your main branch.
  ![Git flow](https://www.gitkraken.com/wp-content/uploads/2021/03/git-flow-4.svg)
  [Source](https://www.gitkraken.com/learn/git/git-flow)

### **Steps for basic Git-flow**:

1.  **Main** branch is only for client not for develop.
2.  Create a **"develop"** branch.
3.  New feature branch -> branch [feature-name].
4.  When the feature is finished, **merge with develop**.
5.  All features are ready, **merge with main**, add a tag/release.
