# Getting Started
[![Pictures-from-ProGit](https://img.shields.io/badge/Pictures%20from-ProGit-yellow.svg)](https://git-scm.com/book/en/v2)

## Version Control
**Version control** is a system that records changes to a file or set of files over time so that you can recall specific versions later. For eg, facebook it has earlier very less features aas compared to today, and so they used to make chnages to their earlier version so that they do not need to write whole code again.<br>

## Local Version Control Systems
<img src="https://github.com/Nehasingh1300/TheOpenSourceGuide/blob/master/Module%202/resources/lvcs.PNG" >
When you copy material from one Operating System to another, this is very basic feature and so it is very tedious and not safe work as your code can be lost or displaced.<br>

## Centralized Version Control Systems
<img src="https://github.com/Nehasingh1300/TheOpenSourceGuide/blob/master/Module%202/resources/cvcs.PNG" >
CVS has one server in which everyone push their code. It has advantage over LVCS that developers are aware about the code present in server but if in any condition the server gets down then no one will be able to push or fetch code.<br>

## Distributed Version Control Systems
<img src="https://github.com/Nehasingh1300/TheOpenSourceGuide/blob/master/Module%202/resources/dvcs.PNG" >
In DVCS, every clients mirror the repository in their local system, so even if server is lost they do not need central repo. They have their code with them.<br>

## Git Basics
**Stream of Snapshot** : Git does not take its data as stream of snapshot, Every time there is commit it compares it's data and with last updated file and only saves thee changes if changes are not made then it will not save the file.

## Git Has Integrity
Git uses a 40-character string composed of hexadecimal characters (0–9 and a–f), which is a called checksum,  SHA-1 hash, whenever you commit any change to git.

## The Three States
<img src="https://github.com/Nehasingh1300/TheOpenSourceGuide/blob/master/Module%202/resources/threestage.PNG" ><br>
**Committed** : Data is stored in local database<br>
**Modified** : Changed file but not committed to data base.<br>
**Staged** : Pushed your code to current version of your database to next commit snapshot.<br>

## The Command Line
There are plenty of commands for git commands which are easy to use and though we have GUI also but if you know how to use command line than it is far easier for you to work with GUI.

## Installing Git
Even if it’s already installed, it’s probably a good idea to update to the latest version. You can either install it as a package or via another installer, or download the source code and compile it yourself.<br>
There are plenty of videos out there which can also help you better installing ubuntu. 
### Installing on Linux
Open your terminal and type<br>For Fedora :
```
sudo yum install git-all
```
For Debian :
```
sudo apt-get install git-all
```
## First-Time Git Setup
### Your Identity
Set up your identity
```
 git config --global user.name "John Doe"
 git config --global user.email johndoe@example.com
```
### Your Editor
Configure the default text editor that will be used when Git needs you to type in a message. If not configured, Git uses your system’s default editor.
Emacs :
```
 git config --global core.editor emacs
```
## Checking your Settings
If you want to check your settings, you can use the git config --list command to list all the settings Git can find at that point:
```
 git config --list
```
