# Git Practice Labs

## Overview
This project demonstrates hands-on Git skills including repository initialization, committing changes, branching, merging, and preparing for pull requests.  
All steps were performed manually in the terminal to simulate real-world Git workflows.

---

## Step 1: Create Project Directory and Initialize Git Repository
Create a new project folder and initialize a Git repository.


mkdir ~/projects/git-practice
cd ~/projects/git-practice
git init

![Terminal window showing directory creation and git initialization commands. User navigates to projects/git-practice directory and runs git init command, which displays output initializing an empty Git repository with details about the .git directory.](images/git-init.png)

## Step 2:Create First File and Commit

Create a text file, stage it, and make the first commit.

echo "Hello World" > file1.txt
git add file1.txt
git commit -m "Add file1.txt"

![Terminal showing creation of file1.txt containing Hello World, staging the file with git add, and committing with message Add file1.txt. Output shows commit hash and confirmation that one file was created.](images/create-first-file-commit.png)

## Step 3: Create a Feature Branch and Modify File

Create a new branch and add feature content to the file.

echo "Hello World" > file1.txt
git add file1.txt
git commit -m "Add file1.txt"


![Terminal showing git branch command to create feature-branch, git checkout command to switch to the new feature branch, and echo command appending feature content to file1.txt. Output confirms successful branch creation and file modification.](images/create-featurebranch-modify-file.png)

## Step 4: Merge Feature Branch into Main

Switch back to the main branch and merge changes.

git checkout master
git merge feature-branch

![Terminal showing git checkout command switching to master branch and git merge command merging feature-branch. Output indicates successful fast-forward merge integrating feature-branch changes into master branch.](images/merge-featurebranch-into-master.png)

## Step 6: Add Remote Repository and Push to GitHub

Connect the local repository to GitHub and push changes

git remote add origin https://github.com/gregodprogrammer/git-practice.git
git add README.md file1.txt
git commit -m "Project 2: Git practice labs"
git push -u origin main

