---
layout: post
categories: github
---

* Add Remote Workspace
`git remote -v`

* Add Upstream
`git remote add upstream https://github.com/MicrosoftDocs/mslearn-tailspin-spacegame-web.git`

### Git Command Summary
#### Category - Repository
* Create a Git repository `git init`

* Download a remote repository `git clone`

#### Branch
* Create/Switch to a branch `git checkout`

    eg `git checkout -b build-pipeline`

    The `-b` argument specifies to create a new branch if it doesn't exist. Omit the `-b` argument when you want to switch to an existing branch.

    eg `git checkout -b feature/home-page-text`

    Add prefix before branch name as convention like `feature/<branch-name>` or `bugfix/<bug-number>`

* Check current branch `git branch -v`

* Delete a branch `git branch -d`

#### Stage and Commit Changes
* See which files have been changed `git status`

* Stage files to commit `git add`

    eg `git add azure-pipelines.yml templates/build.yml`

* Commit files to a branch `git commit`

    eg `git commit -m "Add build tasks"`

    The -m argument specifies the commit message.

    [About Git Commit Message](https://chris.beams.io/posts/git-commit/)

#### Remote Synchronization
* Download a branch from a remote repository `git pull`

    eg `git pull origin master`

* Upload a branch to a remote repository `git push`

    eg `git push origin build-pipeline`

* Submit pull request to merge branch

    1. On GitHub web repo, navigate to branch tag.

    2. Next to desired branch, select `Create Pull Request`

    [Reference](https://docs.microsoft.com/en-us/learn/modules/implement-code-workflow/5-push-a-change#submit-a-pull-request)

    3. Optionally add pull request policies to protect the master branch

* Merge >=2 dev Changes `git merge`

    [Offical git merge doc](https://git-scm.com/docs/git-merge)

    [git merge vs GitHub Pull Request](https://softwareengineering.stackexchange.com/a/304926)

    used by git pull to incorporate changes from another repository

    In below example, current branch is `master` while `topic` branched from `master` (**E**)

    ```
          A---B---C topic
         /
    D---E---F---G master
    ```

    Running `git merge topic` applies `topic` changes (**A** to **C**) on `master` (**G**) and create **H**.

    ```
          A---B---C topic
         /         \
    D---E---F---G---H master
    ```

    1. Checkout/Switch to master branch to check for udpates

        `git checkout master`

        `git pull origin master`
    
    2. Checkout/Switch to specified branch (like feature branch)

        `git checkout feature/home-page-text`
    
    3. Merge current branch to master

        `git merge master`

### GitHub Branching Workflow

![github-brancing-workflow-1](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-1.png)

![github-brancing-workflow-2](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-2.png)

![github-brancing-workflow-3](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-3.png)

![github-brancing-workflow-4](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-4.png)

![github-brancing-workflow-5](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-5.png)

![github-brancing-workflow-6](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-6.png)

![github-brancing-workflow-7](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-7.png)

#### Branching Strategies
[Reference](https://docs.microsoft.com/en-us/learn/modules/implement-code-workflow/10-summary#implement-branch-strategies)

* Feature Branch Workflow

* Gitflow Workflow

* Forking Branch Workflow

### GitHub Badge
