Great, I hope all of you were able to get git installed. If not I'm available for questions, or help.

## A basic git workflow
Ok, now let's get started with a basic workflow using git. I really hope all of you are familiar with the command line because that will be a big part of this course. (Windows users, your commands will be the same if you are using git bash).

Here is a list of the things we are about to do.

1. create a project
2. initialize a git repo
3. add changes to be commited
4. commit changes
5. push to GitHub

Which will look like this in the command line:

```bash
# initialize repo
git init

# add files, code, etc

# track changes with add
git add -A

# commit changes
git commit -m "Init commit"

# see what you've done
git status
git log -v
```

Now, if we have a GitHub account and a remote repo ready to go, we can use the following:

```bash
git remote add origin https://github.com/kissmygritts/git-basics.git
git branch -M main
git remote -u origin main
```