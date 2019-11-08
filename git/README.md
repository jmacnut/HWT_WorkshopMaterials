# Git & GitHub 101
- Meetup for this event: https://www.meetup.com/Honolulu-Women-in-Technology-Meetup-Group/events/265672112/

## Introduction

### Git vs. GitHub
- **Git** is a distributed version control system that is free to use. Version control software keeps track of revisions to the codebase. "Distributed" means that Git keeps a copy of the entire codebase on each developer's machine. Git is available on most operating systems, including Mac OS, Linux, and Windows.
- **GitHub** is a software service that uses Git and hosts copies of a codebase and its revision history in the form of a repository. Usually, a single GitHub repository contains the entire codebase for a software project. However, it is also possible to divide a large project into multiple GitHub repositories.

### Why use Git?
- Git makes life much easier for you and your teammates! Instead of having to remember what files you changed, then sending your teammates a copy of those files, you can say goodbye to worry and just `git push` your changes. Your teammates can then retrieve those changes later with `git pull` when they need it.
- Git helps your productivity by relieving stress: You don't have to get upset at future you for deleting rather important code. You can just go back to that point in time and reverse the changes made, if needed.

### Why use GitHub?
- GitHub provides free unlimited public and private repositories, with no limit on the number of collaborators for a public repository, and up to 3 collaborators for private repositories. That's quite a lot for free and more than enough to get started.
- GitHub gives you a chance to showcase your work to future employers and the world via public repositories. And you can always start out with a private repository before making it public.
- GitHub has become a social network of sorts, allowing all kinds of developers to share their work, meet, discuss, or collaborate.

### What is a terminal and why use it?
- A terminal or command-line interface (CLI) is an interface that accepts commands issued to the operating system, as opposed to clicking on buttons using an application to tell the computer what to do. In short, you type commands into a prompt (like a text message input) to execute commands that can copy files, view files in a directory, and download files from the Internet, etc.
- Knowing your way around a terminal is crucial not just for learning Git but for using other useful software tools as well. More on that later!

## Getting Started

### Terminal Setup
1. The Terminal app comes pre-installed for Mac users and Windows users can use Git for Windows: https://gitforwindows.org/

### GitHub Setup
1. Create a GitHub account: https://github.com/join
1. **Fork** this repository by clicking "Fork" in the top right-hand corner: https://github.com/honoluluwomenintech/WorkshopMaterials
    - The process of forking creates a new copy of the forked repository at a new **remote** (like an "address" for where the code lives)
    - That new remote will be your GitHub username and will live at: https://github.com/your-username-here/WorkshopMaterials
1. After forking and being redirected to the new copy, click on the green "Clone or download" button and copy the HTTPS link (it'll be the same as the URL but you'll see `.git` at the end)

### Git Setup
1. Download Git for your operating system: https://git-scm.com/downloads
1. Install Git by following the installation instructions
1. Have the terminal ready and you're all set!

## Git Commands

Now we're ready to use Git in the terminal. Please [refer to the workshop PDF](https://github.com/honoluluwomenintech/WorkshopMaterials/blob/master/git/hwt_study_git_intro.pdf) to start learning some Git commands.

### Examples of commonly used git commands
    - to start a git repo (once git is set up on your desktop)
```git init ```

    - to stage files to be commited to repo
```git add myfile.txt```
    
    - to commit any changes made to your file (with a message)
```git commit -m 'i added a new section at the end of the file'```

    - to pull repo from your remote server to your local computer (master branch)
 ```git pull origin master```
    
    - to push repo from your local computer to remote server (master branch)
 ```git push origin master```
