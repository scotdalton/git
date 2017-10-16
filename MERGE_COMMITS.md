# Merge Commits

Merge finds the common ancestor between `master` and `your-branch` and creates
a new merge commit by doing a three way merge from the snapshot of code in the
common ancestor, the snapshot of the latest code in `master` and the snapshot of
the latest code in `your-branch`.

- it only happens on non fast-forward merges
- by default merge always tries to fast-forward


Merge commits cloud the view of history by adding commits that don't actually contain changes.

```sh
~> git merge --no-ff son
~> git co daughter
~> git merge merge-commits
~> git co merge-commits
~> git merge --no-ff daughter
```
