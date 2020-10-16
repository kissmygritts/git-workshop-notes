`git commit` is used to take a snapshot of your staging area. Anything that is unstaged, not tracked, will not be included in this commit. `git commit -m "Commit message"` is generally how you want to do this. If you don't use the `-m` option git will open your default editor for you to create a commit message. This is usually a program called vim or vi. 

After the commit is created you'll see which branch you committed, the SHA-1 checksum (or git hash) assigned to this commit, how many files were changed, and the stats about what was added or removed.

## Viewing the commit history
Viewing the commit history is a very useful tool. We will revisit this several times throughout the workshop.

The basic command is `git log` which will show the verbose output of your git history. Let's review several of the options for the Pro Git book with our own repo.

```bash
git log

git log -p -2

git log --stat

git log --pretty=oneline

git log --format:"%h - %an, %ar : %s"

git log --pretty=format:"%h %s" --graph
```

There are many options that can be used with `git log` many of the more interesting ones come into play once you've been using git for awhile.

## Walk through the commit history

This is a risky operation. Make sure you've pushed to GitHub just in case you make a mistake!

```bash
# move back to a specific commit
git checkout <commit hash>

# view logs
git log --oneline
git log --all --oneline

git status

# go back to the top
git checkout master
```