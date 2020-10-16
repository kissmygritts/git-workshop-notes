The `git status` command is used to determine the state of each file in your repo. Files are either tracked or untracked. 

Tracked files are files that were in the last snapshot - files git knows about. These files can be: 
- unmodified
- modified
- staged

Untracked files are everything else. Any files that were not in the last snapshot and are not in the staging area.

![[lifecycle.png]]

Files become tracked by using `git add`. This lets git know about files in your directory. Once tracked files can switch between any of the unmodified, modified, and staged states. 
- `git add` tracks files or stages modified files
- `git commit` creates a new snapshot of your file system based on the currently tracked files

*It is impossible to demonstrate about `git status` without also using `git commit` or `git add`. We'll talk more about those moving forward.*

