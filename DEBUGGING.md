# Debugging

## Blame

You've found a bug and want to know the when/why/who of its introduction.

```sh
~> git blame code
```

## Grep

Search for a string or regex in the working directory.

```sh
~> git grep "bad" code
```

## Bisect

Binary search through your commits to identify the bad commit.

```sh
~> git bisect start
~> git bisect bad HEAD
~> git bisect good origin/master
~> git grep "bad" code
~> git bisect good
~> git grep "bad" code
~> git bisect bad
~> git grep "bad" code
~> git bisect bad
~> git bisect reset
```
