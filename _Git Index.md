# Grad 778: Elements of Research Computing
## Module: Version Control with Git & GitHub

## Outline
A quick outline of the topics we will cover. Each section should link to a note with more information.

0. [[Getting started with git]]
	1. [[Installing git macOs]]
	2. [[Installing git on Windows]]
	3. [[first time git configuration]]
	4. [[git tooling]]
	5. [[A quick tour of GitHub]]
	6. [[Git resources]]
	7. [[attendance assignment]]
	8. [[Workshop notes]]
1. Git Basics
	1. [[Getting started with git]]
	2. [[Get help with git]]
	3. [[cloning a repo]]
2. Working with and understanding git
	1. [[What is a repository]]?
	2. [[git status]]
	3. [[git add]]
	4. [[Ignore files with gitignore]]
	5. [[git commit]]
3. Collaborating with others
	1. [[Create a fork, clone, pull requests]]
	2. [[How to complete the attendance assignment]]
4. git branch & branching workflows
	1. [[Create a new branch]]
	2. Merge conflicts
5. troubleshooting git

## A brief intro to git
Git is a version control system (VCS) for tracking changes in any set of files. It is used to help coordinate work between programmers/designers/developers/etc. Everyone in a team can work on the same code at the same time.

As an example you and a lab partner are working on a programming assignment. Before git the workflow might look like using a shared Dropbox folder, or emailing files back and forth. But what happens when you both edit the same thing and try and save at the same time? Your guess is as good as mine. With git you can create a remote repository and each contribute code independently to same repo. Each of you have an exact copy of the code as it exists in the remote repo. When conflicts do arise there are tools to help resolve them.

![[git.png]]

Git doesn't need to be complicated. Everything is a variation on this simple workflow:
1. initialize a repo
2. add code, make changes 
3. stage changes for commit - [[git add]]
4. commit changes - [[git commit]]
5. push to remote repo

This is what we will focus on during this workshop. Every other *advanced* git workflow still contains these steps, with a few others thrown in just to confuse us.

### Some things to know
This workshop will be a lot easier if you have some experience with the command line. I'll be typing almost everything in the terminal so if you don't know the command line well you will be fine. 

Programming isn't a prerequisite for this workshop, however I will be using some examples from R or JavaScript or Python. The contents of these files doesn't matter. All we car about is tracking the changes in the contents of these files. 

Markdown is a simple markup language that I will use extensively throughout the workshop. Markdown is a tool widely adopted when working with git. These notes are written in Markdown.

A quick list of the things we will use in this course:
- command line (bash, zsh, git bash on windows)
- GitHub - see [[A quick tour of GitHub]]
- Visual Studio Code
- a Text editor
- 

## A little about me
My name is Mitch Gritts and I work as a developer/biologist at NDOW. I use git nearly everyday but often have to Google anything beyond the basic workflow

## TAs

## Participants

- Carissa Romero

## These notes
[[Workshop notes]] for more information about these notes

