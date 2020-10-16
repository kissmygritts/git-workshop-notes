A quick overview of how to use git. You don't need to following along with the video if you don't want to. I'll provide the commands I run below so you can run them at your own pace.

Remember the workflow looks like this:
1. Initialize a repo
2. create files, modify files
3. stage files, changes for commit
4. commit changes
5. push to GitHub

```bash
# 1. initialize repo
git init

# 3. stage files for commit
git add -A

# 4. commit changes
git commit -m "Commit message"
```

Since we are starting with a new repo we will have a few additional steps before pushing to GitHub. The first step is to create a repo on GitHub.

Then do the following (GitHub will prompt you to do this)

```bash
# add a remote branch
git remote add origin https://github.com/kissmygritts/[repo-name].git

# change the name of our default branch
git branch -M main

# push to the remote branch
git push -u origin main
```

And that is it! I'll probably walk through this a couple of times.