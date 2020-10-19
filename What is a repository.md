A `repository`, often shortened to `repo`, is a directory of files and folders associated with a project. For example, everything in the file structure below is part of a git repository:

```tree
.
├── .git
├── README.md
├── scripts
│   ├── R
│   │   ├── add.R
│   │   ├── divide.R
│   │   ├── main.R
│   │   ├── multiply.R
│   │   └── subtract.R
│   ├── javascript
│   │   ├── add.js
│   │   ├── another.js
│   │   ├── main.js
│   │   └── root.js
│   └── python
│       └── main.py
└── secrets.md

4 directories, 12 files
```

The biggest indicator that this is a git repo is the `.git` folder. This is a folder created by git used to track the history of the project.

## Commits
The file history appears as a series of snapshots called `commits`. Commits exist as a linked-list relationship - a *tree* ([you can think of it as a graph if that helps](http://think-like-a-git.net/sections/graph-theory.html)). Creating a commit is a two-step process. First use `git add` to add files to the staging area. Then use `git commit` to create a snapshot of the repository.

## Branches
These commits can be organized into multiple `branches`. [Branches](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell) allow you diverge from the main line of development and continue work, on new features or bugs, without derailing your *main* branch. Git creates a branch by default called *master* or *main* (see [[first time git configuration#Default branch name]]). Create new branch with `git checkout -b branch_name` where `branch_name` is the name of the branch you want to create.

Every commit belongs to a branch. *Main* or *master* is a branch, your remote repositories on GitHub are branches (remote branches). View all branches with `git branch -v --all`. This might be a helpful hint to remember as we continue the workshop.

![[reachability-example.png]]

## History
View the history of a repository with `git log`. An example of the output for `git log` looks a little like this:

```
|\  
| * d535c9d is definitely an elk
| *   af6c13c Fix merge conflict to elk
| |\  
| | * 0c147bd Change to elk in main
| * | 03077a8 Change to cat
| |/  
* | 11727ac Add add.js
* | 42e5cdb Change to snake
|/  
* 593d110 Start animal branching conflicts
*   c8ecd86 Fix color change merge conflict
|\  
| * 1c453f5 Change color to orange
* | 5054c5c Change color to red
|/  
* 36c376c Begin merge conflicts
* cf251b0 Fix parameter order in operations
*   38e79b2 Merge pull request #1 from kissmygritts/feat-math-functions
|\  
| * 0059274 Add divide function in R
| * f25064f Add a subtract function in R
|/  
* 3dd9726 Clean up scripts, create lang files
* bfef2e2 Begin tracking javascript files
* 40d3f48 Update gitignore again
* d7276e9 Update gitignore
* d5a771f Remove secrets.md
* 2738fda Add .gitignore
* cd3b273 End of the day commit
* e4ab518 Delete new-file.md
* ebe26f1 Mistakes were made
* 2cf4b69 Added more R scripts
* c2eb09e Update python scripts
* 0e2c181 Update R scripts
* 604af2e Add scripts
* 31a1faf More changes
* 58e8c5d New file
* 343bcbf Modified readme, added fall 2020
* c99aa58 Init commit
```

Each `*` in this log is a commit. This is the complete history of a git repository. We can navigate to any point within this history, to a specific snapshot, by referencing the git hash (the 7 digit hexidecimal ID). This example includes several branches, indicated by the `|, \, /` characters within the log.

## Moving forward
This section laid out some important concepts that we will work through in the remainder of the workshop. An important thing to remember is experiment. The beauty of git is that we can go back through our commit history to undo (or redo) any work we've done. At this stage of learning git it is hard to mess anything up! We are working with example repositories. Nothing here is so important that it can't be deleted. When working on your own code repositories more caution is warranted. If I feel like I might mess something up, or want to experiment I'll push to GitHub, create a new branch, then do the experiments in the new branch. This gives me confidence that I'll likely never screw up too badly.