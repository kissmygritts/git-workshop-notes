## Outline
A quick outline of the topics we will cover. Each section should link to a note with more information.

0. [[Getting started with git]]
	2. [[Installing git macOs]]
	3. [[Installing git on Windows]]
	4. [[first time git configuration]]
	5. [[git tooling]]
	6. [[A quick tour of GitHub]]
	7. [[Git resources]]
	8. attendance assignment
1. Git Basics
	1. [[Getting started with git]]
	2. [[Get help with git]]
	3. [[cloning a repo]]
2. More details about git commands
	1. [[git status]]
	2. [[git add]]
	3. [[git commit]]
	4. git log
	5. git push
	6. git clone
3. Forking
4. git branch & branching workflows
5. Merge conflicts
6. troubleshooting git

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

## These notes
These notes will live on GitHub and act as a living version of this course. As I find additional content or resources I'll add them to the notes and push the changes to GitHub.

I'm using an application called Obsidian to write and display these notes throughout the workshop. It works on any platform and allow you to have your own local copy of these notes. 

We'll talk about [[cloning a repo]] later (specifically cloniing these notes). But if you can't wait the URL for this repo is `https://github.com/kissmygritts/git-workshop-notes.git`