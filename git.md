# git
git help git

## ressources
- [The Odin Project](https://www.theodinproject.com/) 
[git introduction](https://www.theodinproject.com/lessons/foundations-introduction-to-git) 
[git basics](https://www.theodinproject.com/lessons/foundations-git-basics)
- [boot.dev](https://boot.dev) 
[learn git](https://www.boot.dev/courses/learn-git) 
[larn git 2](https://www.boot.dev/courses/learn-git-2)

## high level commands - porcelain
`git status`
`git add`
`git commit`
`git push`
`git pull`
`git log`

## low level commands - plumbing
`git apply`
`git commit-tree`
`git hash-object`

## config
`git config get user.name`
`git config get user.email`
`git config set --global user.name "github_username_here"`
`git config set --global user.email "email@example.com"`
`git config list --local`
`git config get <key>`
`git config unset <key>`
`git config unset --all example.key`
`git config remove-section <section>`

`git config set --global init.defaultBranch master`
`git config set --global init.defaultBranch main`
`git config set pull.rebase false`

### config locations
system: /etc/gitconfig, a file that configures Git for all users on the system
global: ~/.gitconfig, a file that configures Git for all projects of a user
local: .git/config, a file that configures Git for a specific project
worktree: .git/config.worktree, a file that configures Git for part of a project


create git repository
`git init`

`git commit -m "your message here"`

`git --no-pager log -n 10`

see the contents of a commit
`git cat-file -p <hash>`

## branch
`git branch`

rename branch
`git branch -m oldname newname`

create branch
`git branch my_new_branch`
`git switch -c my_new_branch`


switching branches
`git switch branchname`

or, the old way:
`git checkout branchname`

`delete branch`
`git branch -d branchname`


## log
- [docs](https://git-scm.com/docs/git-log)  
`git log --decorate [full|short|no]`
`git log --oneline`
`git log --oneline --graph --all`
`git log --oneline --decorate --graph --parents`


## merge
merge branchname into main  
`git switch main  `
`git merge branchname`  

## rebase
avoid merge commits

To use rebase to bring changes from main onto a current branch. You should never rebase a public branch (like main) onto anything else.  
`git rebase main`

## undo changes
change last commit message (changes commit hash)  
`git commit --amend`

The git reset command can be used to undo the last commit(s) or any changes in the index (staged but not committed changes) and the worktree (unstaged and not committed changes).

The --soft option is useful if you just want to go back to a previous commit, but keep all of your changes. Committed changes will be uncommitted and staged, while uncommitted changes will remain staged or unstaged as before.  
`git reset --soft COMMITHASH`

undo last commit, keep changes  
`git reset --soft HEAD~1`

DANGER!!!
The --hard flag makes your working directory and staging area match the specified commit exactly, discarding any local changes. This is useful if you just want to go back to a previous commit and discard all the changes.  
`git reset --hard COMMITHASH`

## remote
`git remote add <name> <uri>`

fetch files from remote
`git fetch`
`git fetch origin`

merge with branch in remote repo
`git merge [<remote>/<branch>]`

push changes to remote
`git push origin main`

push a local branch to a remote with a different name:
`git push origin <localbranch>:<remotebranch>`

delete a remote branch by pushing an empty branch to it:
`git push origin :<remotebranch>`

`git pull [<remote>/<branch>]`


## squash
Squashing take all the changes from a series of commits and squash them into a single commit.  
`git rebase -i HEAD~n`

## stash
[doc](https://git-scm.com/docs/git-stash)  
`git stash`  
`git stash list`
`git stash pop`
`git stash apply`
`git stash drop`  

Apply the third (0, 1, 2) most recent stash  
`git stash apply stash@{2}`

Remove the third most recent stash  
`git stash drop stash@{2}`

## revert
`git revert`

