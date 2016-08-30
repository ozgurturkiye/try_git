#

# `fetch` vs `pull` differences

`fetch` will download any changes from the remote* branch, updating your repository data, but leaving your local* branch unchanged.

`pull` will perform a `fetch` and additionally `merge` the changes into your local branch.

**What's the difference?** `pull` updates you local branch with changes from the pulled branch. A `fetch` does not advance your local branch.

* This explanation assumes that the current branch is a local branch, and that the branch specified as the argument to `fetch`, `pull`, `merge`, or `rebase` is a remote branch. This is the usual case. `pull`, for example, will download any changes from the specified branch, update your repository and `merge` the changes into the current branch.

Source: http://stackoverflow.com/questions/14894768/in-git-how-is-fetch-different-than-pull-and-how-is-merge-different-than-rebase

