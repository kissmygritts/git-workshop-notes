`git add` tells git to track any files provided. The template for this command is `git add [files]`. The `[files]` portion of this can be any number of things.
- a list of files: `git add file1 file2`
- an extension with a wildcard: `git add *.R`
- a dot `git add .`, which means all files in the current directory
- or no files: `git add -A` where `-A` is a shortcut for all files

`git add` will also add any modified files to the staging area

## A few ways to use `git add`
```bash
# add all files to the staging area
git add .
git add -A

# use the patch option, use the y/n keys to interactively add files
git add -p
git add --patch

# by filename with git add [filename]
git add script.R
git add scripts/*.r
git add scripts
```

## Removing a file
Sometimes you need to remove a file from your repo.

`git rm` will remove files. This is essentially the same as running the `rm` command. It permanently deletes it from you directory. The `---cached` option will only remove it from your repo not from your directory.

```bash
git rm

git rm --cached secrets.md
```
