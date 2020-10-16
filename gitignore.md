`.gitignore` is a special file that allows you to tell git which files in the current directory to ignore. It is very easy to accidentally track and commit files that contain secrets such as passwords or account numbers. Especially when working with remote databases or APIs.

Your best bet is to use a tool like [gitignore.io](gitignore.io) to generate a `.gitignore` file based on best practices. 

Since git tracks your entire history removing files once commited is very difficult. I'll show you an example. 