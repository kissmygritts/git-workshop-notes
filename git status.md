The `git status` command is used to determine the state of each file in your repo. Files are either tracked or untracked. 

Tracked files are files that were in the last snapshot - files git knows about. These files can be: 
- unmodified
- modified
- staged

Untracked files are everything else. Any files that were not in the last snapshot and are not in the staging area.

*see state figure in docs*

Files become tracked by using `git add`. This lets git know about files in your directory. Once tracked files can switch between any of the unmodified, modified, and staged states. 
- `git add` tracks files or stages modified files
- `git commit` creates a new snapshot of your file system based on the currently tracked files

## .gitignore
`.gitignore` is a special file that allows you to tell git which files in the current directory to ignore. It is very easy to accidentally track and commit files that contain secrets such as passwords or account numbers. Especially when working with remote databases or APIs.

Your best bet is to use a tool like [gitignore.io](gitignore.io) to generate a `.gitignore` file based on best practices. 

Removing files once commited is very difficult. I'll try and cover this later in a separate video.

