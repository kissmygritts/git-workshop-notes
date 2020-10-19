The `git status` command is used to determine the state of each file in your repo. Files are either tracked or untracked. 

Untracked files are those that git is unaware of (haven't been added yet) or you intentionally don't want git to track (with something like [[Ignore files with gitignore]]).

Tracked files are files git knows about. These files can be: 
- unmodified - haven't changed since the last commit
- modified - files that have modifications since the last commit
- staged - files that are staged for commit, these files have modifications of some kind

![[lifecycle.png]]

Files become tracked with `git add`. This lets git know about files in your directory. Once tracked files can switch between any of the unmodified, modified, and staged states. 
- `git add` tracks files or stages modified files
- `git commit` creates a new snapshot of your file system based on the currently tracked files

*It is impossible to demonstrate about `git status` without also using `git commit` or `git add`. We'll talk more about those moving forward.*