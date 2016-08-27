# git basic

Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

The Git workflow consists of editing files in the `working directory`, 
adding files to the `staging area`, 
and saving changes to a `Git repository`. In Git, we save changes with a `commit`

Working Directory | Staging Area | Repository 
----------------- | ------------ | ----------
Make changes to files: | Bring changes in to the staging area | Save changes to the repository a a `commit`
1 | 2 | 3

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


For more info: https://www.codecademy.com/learn/learn-git
