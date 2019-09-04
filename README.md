# Git Lab
---

This is a single page website that explains git and some basic examples.

Let's add a gif. Something really cool.

Copy and commit the changes to your repo. Watch the page in all it's glory.

Ok maybe it doesn't fit with the theme of the repo. We may want to undo the 
changes we made.

A `revert` is a special form of `commit` that puts a repository back the way 
it was before a given `commit`. If you haven't noticed by now, git commits are 
referenced by a hash that is unique to the commit. In addition to a hash, the 
last `commit` to a repo is also referenced via `HEAD`. So to revert the last 
commit, we simply issue:

```
➜  test git:(master) git revert HEAD --no-edit 
[master 2c90403] Revert "added something we'll regret"
 Date: Tue Sep 3 17:00:09 2019 -0500
 2 files changed, 15 insertions(+), 13 deletions(-)
 rewrite README.md (75%)
➜  test git:(master)
```

In the command above, we used the `--no-edit` flag to indicate that we want to 
use the default commit message. This will, in most implementations of the `git`
client, use the message `Revert '<Reverted Commit Message Here>'`. Without the
`--no-edit` flag, `git` will open your default git editor and let you change
the message.

When you are done, you will need to push your revert to the master with
`git push origin master`.

After everything has been pushed, copy the contents of `4_branch_creation` and
follow the instructions to continue.