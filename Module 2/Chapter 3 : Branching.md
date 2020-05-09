# Branching
When you don't want to mess with other's work in the main line of work then you shift a little bit to other path (called branches), where you can work the way without worrying about breaking other's code.

## Branching in nutshell
Git stores commit as snapshot of the difference of last commit and with that information about the author like, email, name, time, commit number and other information. Default branch of Git is **master**.

## Creating a new branch
When you create a branch then the pointer is shifted to that branch and from that branch commit history is bring stored.<br>
**Creating a new branch**<br>
```
git branch branch-name
```
But when you check which branch you are working on, it will show **master**. Use the command below to check your branch.
```
git branch 
```
For going to branch you made, and working init, you will need to **checkout** to it and then work according.
```
git checkout branch-name
```
You can make as many branch you want according to the number of developers you have.
