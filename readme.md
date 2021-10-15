# Merge Experiment

Goal: check the merge with upstream needs `merge commit` or `rebase commit`, instead of `squash commit`
when managing a fork repo.

Only merge/base commit allows the original commit is preserved. otherwise the next sync will cause git merge conflict.

How to enable this:
[Github doc](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/configuring-pull-request-merges/configuring-commit-rebasing-for-pull-requests).


This is the upstream merge experiment, parent repo.

See github.com/incfly/merge-exp-child

