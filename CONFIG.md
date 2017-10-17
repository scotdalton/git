# Config

Use the `.gitconfig` to make `git` your own.

```sh
~> cat ~/.gitconfig
[user]
 name = Scot Dalton
 email = scotdalton@gmail.com
[core]
 editor = vim
[merge]
 tool = vimdiff
[alias]
 s = status -sb
 lg = log --decorate --color --oneline --graph
 nff = merge --no-ff
 co = checkout
 amend = commit --amend
 staged = diff --staged
 puhs = push
[push]
 default = simple
[branch]
 autosetuprebase = always
 ```

 or

 ```sh
 ~> git config -l
 user.name=Scot Dalton
 user.email=scotdalton@gmail.com
 core.editor=vim
 merge.tool=vimdiff
 alias.s=status -sb
 alias.lg=log --decorate --color --oneline --graph
 alias.nff=merge --no-ff
 alias.co=checkout
 alias.amend=commit --amend
 alias.staged=diff --staged
 alias.puhs=push
 push.default=simple
 branch.autosetuprebase=always
 core.repositoryformatversion=0
 core.filemode=true
 core.bare=false
 core.logallrefupdates=true
 core.ignorecase=true
 core.precomposeunicode=true
 ```
