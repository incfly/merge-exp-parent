# Merge Experiment

Goal: check the merge with upstream needs `merge commit` or `rebase commit`, instead of `squash commit`
when managing a fork repo.

Only merge/base commit allows the original commit is preserved. otherwise the next sync will cause git merge conflict.

How to enable this:
[Github doc](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/configuring-pull-request-merges/configuring-commit-rebasing-for-pull-requests).


This is the upstream merge experiment, parent repo.
See github.com/incfly/merge-exp-child

## Experiment

- child:main, good merge, `merge commit`, preserving the commit., https://github.com/incfly/merge-exp-child/pull/1
- child:bad-tip, bad merge, `squash merge`, single commit, https://github.com/incfly/merge-exp-child/pull/2
- add new commit here.
- do git pull && merge in child again in above two branches, the bad-tip sees conflicts.

