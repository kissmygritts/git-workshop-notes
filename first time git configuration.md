Now, let's cnfigure a few global parameters. Find comprehensive review of [first time git setup here](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)

Git will use information about you, your machine, or your aliases within every commit. We'll start with your username and email.

```
git config --global user.name "your name"
git config --global user.email "your_email@email.com"
```

I've always used the same username and email here as I do for my GitHub credentials. We can change this later.

## Default branch name
**Requires Git version 2.28 or greater**.

By default git uses `master` as the name of the default branch. In the interest of diversity, equity, and inclusion we can rename this branch to `main`. Really, we can name it whatever we want, but let's stick with conventions. 

```
git config --global init.defaultBranch main
```

I am currently working with git version 2.27 so I cannot run this command for you. For those of you that are also on older versions of git like me there is a more manual work around. I'll show you when we get to that part.