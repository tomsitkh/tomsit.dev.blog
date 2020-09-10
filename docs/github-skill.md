---
categories: github
---

* Add Remote Workspace
`git remote -v`

* Add Upstream
`git remote add upstream https://github.com/MicrosoftDocs/mslearn-tailspin-spacegame-web.git`

* Submit pull request to merge branch

### Git Command Summary
#### Category - Repository
* Create a Git repository `git init`
* Download a remote repository `git clone`

#### Branch
* Create/Switch to a branch `git checkout`

eg `git checkout -b build-pipeline`

The `-b` argument specifies to create a new branch if it doesn't exist. Omit the `-b` argument when you want to switch to an existing branch.

* Check current branch `git branch -v`

* Delete a branch `git branch -d`

#### Stage and Commit Changes
* See which files have been changed `git status`

* Stage files to commit `git add`

eg `git add azure-pipelines.yml templates/build.yml`

* Commit files to a branch `git commit`

eg `git commit -m "Add build tasks"`

The -m argument specifies the commit message.

#### Remote Synchronization
* Download a branch from a remote repository `git pull`

eg `git pull origin master`

* Upload a branch to a remote repository `git push`

eg `git push origin build-pipeline`

### GitHub Branching Workflow

![github-brancing-workflow-1](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-1.png)

![github-brancing-workflow-2](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-2.png)

![github-brancing-workflow-3](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-3.png)

![github-brancing-workflow-4](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-4.png)

![github-brancing-workflow-5](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-5.png)

![github-brancing-workflow-6](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-6.png)

![github-brancing-workflow-7](https://docs.microsoft.com/en-us/learn/azure-devops/implement-code-workflow/media/2-github-paths-7.png)
