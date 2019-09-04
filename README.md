# Git Lab
---

This is a basic website that shows some simple git commands and examples.

Once you've copied the contents of this folder into your repository, open your command line and navigate to this folder. Run `git status` to see the currently modified files: 

```
➜ lab git:(master) git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	README.md
	index.html

nothing added to commit but untracked files present (use "git add" to track)
➜ lab git:(master)
```

You can then add the changes to the list of changes to be committed with `git add <filename>`:

```
➜  lab git:(master) git add README.md
➜  lab git:(master) git add index.html
➜  lab git:(master) git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   README.md
	new file:   index.html

➜  lab git:(master)
```

Finally, you can commit the changes with `git commit -m "initial commit"`:

```
➜  lab git:(master) git commit -m "initial commit"
[master (root-commit) 55897b9] initial commit
 2 files changed, 34 insertions(+)
 create mode 100644 README.md
 create mode 100644 index.html
➜  lab git:(master) git status
On branch master
nothing to commit, working tree clean
➜  lab git:(master)
```

If your repository is also remote, you can push the changes with `git push origin master`:

```
➜  lab git:(master) git push origin master
Warning: Permanently added the RSA host key for IP address '140.82.113.3' to the list of known hosts.
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.15 KiB | 1.15 MiB/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To github.com:username/git_lab_test.git
 * [new branch]      master -> master
➜  lab git:(master)
```

That concludes the first lab! Feel free to open the repository in a web browser and view it if you're using GitHub or another web service.

When you're ready to continue, copy the contents of the `2_update_website_content/` folder (so that `README.md` is in the root of the repo directory). This will overwrite work in this directory, but that's ok! We've got it all versioned, after all...
