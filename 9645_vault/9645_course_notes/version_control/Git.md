
## What is Git?
Git is a source or version control software created by [Linus Torvalds](https://en.wikipedia.org/wiki/Linus_Torvalds) the creator of [Linux](https://en.wikipedia.org/wiki/Linux) It allows multiple people to work on any code or text based project and manage changes made by one ore more users.

## What is Github?
[Github](https://github.com/) is a software as a service platform owned by Microsoft which hosts Git Repositories, essentially a cloud storage platform for code.

## What is Github Codespaces?
[Github Codespaces](https://github.com/features/codespaces) is a cloud development platform run by github, it hosts an online version of Visual Studio code so that you can code in the cloud without installing VSCode locally on your device, it can be used on anything that can run a modern browser including devices such as ipads.

### Options for using Git
1. Git Command Line Interface (CLI)
2. Github Desktop - a graphical user interface for github
3. VSCode Source Control plugin (installed by default)

### How to use the Git CLI

#### Setting your username and email
``` shell
git config --global user.name yourusername
git config --global user.email youremail@yourdomain.com
```
#### Cloning an existing repository
``` shell
cd <directory where you want the project cloned>
git clone <URL>
```
#### Making a new repository
``` shell
mkdir example
cd example
git init
```
#### Committing to a repo
``` shell
git stage .
git commit -m "describe what you changed"
git push
```