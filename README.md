# git basic

> Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

The Git workflow consists of editing files in the `working directory`, 
adding files to the `staging area`, 
and saving changes to a `Git repository`. In Git, we save changes with a `commit`

Working Directory | Staging Area | Repository 
----------------- | ------------ | ----------
Make changes to files: | Bring changes in to the staging area | Save changes to the repository a `commit`
1 | 2 | 3

About file status : Adding Changes ($ git add `FILE`)

![git_advice]
(https://github.com/ozgurturkiye/try_git/raw/master/git_advice.png)


# Summary

- Git is the industry-standard version control system for web developers
- Use Git commands to help keep track of changes made to a project:
 - `git init` creates a new Git repository
 - `git status` inspects the contents of the working directory and staging area
 - `git add` adds files from the working directory to the staging area
 - `git diff` shows the difference between the working directory and the staging area
 - `git commit` permanently stores file changes from the staging area in the repository
 - `git log` shows a list of all previous commits

# Three different ways to backtrack in Git.
`git checkout HEAD filename:` Discards changes in the working directory.

`git reset HEAD filename:` Unstages file changes in the staging area.

`git reset SHA:` Can be used to reset to a previous commit in your commit history.


# Branch

> Git branching allows users to experiment with different versions of a project by checking out separate branches to work on.

## The following commands are useful in the Git branch workflow.

- `git branch:` Lists all a Git project's branches.
- `git branch branch_name:` Creates a new branch.
- `git checkout branch_name:` Used to switch from one branch to another.
- `git merge branch_name:` Used to join file changes from one branch to another.
- `git branch -d branch_name:` Deletes the branch specified.


# Teamwork

> A remote is a Git repository that lives outside your Git project folder. Remotes can live on the web, on a shared network or even in a separate folder on your local computer.

> The Git Collaborative Workflow are steps that enable smooth project development when multiple collaborators are working on the same Git project.

## We also learned the following commands

- `git clone:` Creates a local copy of a remote.
- `git remote -v:` Lists a Git project's remotes.
- `git fetch:` Fetches work from the remote into the local copy.
- `git merge origin/master:` Merges origin/master into your local branch.
- `git push origin <branch_name>:` Pushes a local branch to the origin remote.
- `git remote add origin <https://github.com/user/repo.git>:` Set a new remote
- `git remote set-url origin <https://github.com/USERNAME/OTHERREPOSITORY.git>:`changes an existing remote repository URL. 

> Git projects are usually managed on Github, a website that hosts Git projects for millions of users. With Github you can access your projects from anywhere in the world by using the basic workflow you learned here.


# git collage
![git-collage]
(https://github.com/ozgurturkiye/try_git/raw/master/git_collage2.jpg)


For more info: https://www.codecademy.com/learn/learn-git

git - the simple guide : http://rogerdudler.github.io/git-guide/
