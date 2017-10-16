# Time Travel

## Amend

Amending allows you to change the history of your last commit

`git commit --amend`

## Rebase

Rebasing allows you to change the history of your branch by replaying your changes
on top of the branch you're rebasing from. It help makes your git repo a baobab tree.

Interactive rebasing is very powerful
  - update the order of your commits
  - remove unnecessary commits
  - amend any of your commits
  - add more commits
  - squash/fixup commits
  - reword your commit messages

### Rules/Recs

- don't rebase `master`
- if you're sharing a branch with a friend, talk to each other
- make rebasing easy
  - short lived branches
  - informative commit messages
  - atomic commits
