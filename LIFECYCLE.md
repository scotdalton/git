# Lifecycle

## Update the Code

```sh
~> echo 'working directory/index' >> lifecycle
~> echo 'another line' >> lifecycle
# stage some changes
~> git add -p lifecycle
```

## Working Directory

Your files

```sh
# diff between what's in your working directory and the Index
~> git diff -- lifecycle
~> git stash -p -- lifecycle
~> git co -- lifecycle
```

## Index

Your "staged" files

```sh
# diff between what's in the staging area and the HEAD snapshot
~> git diff --staged -- lifecycle
~> git reset -p -- lifecycle
```

## HEAD

Your last commit

```sh
# shows the last commit
~> git show HEAD
```

## Remote Reference

A local copy of what the remote repository looks like

```sh
# diffs between the working directory and the local
# reference to the remote repository
~> git diff origin/lifecyle
```

## Remote Repository

The actual remote repository

```sh
# gets from the remote repository and puts it in
# the local reference to the remote repository
~> git fetch origin lifecyle
```
