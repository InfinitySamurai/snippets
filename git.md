# Git

## Simple stuff

- Clone a repo `git clone <repo url>`
- Pull changes from git `git pull`
- Push changes to git `git push`
- Commit changes `git commit -am "<insert commit message here for all changed files>"`
  - There are different ways of commiting, if you want more detail, might not want to use the -m flag and write your message in an actual editor

## Branches

- List local branches `git branch`
- List all branches including remote ones `git branch -a`
- Checkout a branch `git checkout <branchname>`
- Create a new branch from current head `git checkout -b <new branch name>`
- Delete a branch if it's merged into the branch you're currently on `git branch -d <branchname>`
- Delete a branch regardless of it's been merged `git branch -D <branchname>`

  - Note this can be undone, When you delete it, it will give you a hash of the commit which you can use to check it out again

  - > `git branch -D dontDeleteBranch`

    > `Deleted branch dontDeleteBranch (was bcef639)`

    > `git checkout bcef639`
