# Git Teamwork

`git clone remote_location clone_name`

`remote_location`: could be a web address, or a filepath.

`clone_name` is the name you give to the directory in which Git will clone the repository. 

`git remote -v`:a list of a Git project's remotes

- Git automatically names this remote origin, because it refers to the remote repository of origin. However, it is possible to safely change its name. 
 - origin    /home/ccuser/workspace/curriculum/science-quizzes (fetch)
 - origin    /home/ccuser/workspace/curriculum/science-quizzes (push)

- `git fetch`: An easy way to see if changes have been made to the remote and bring the changes down to your local copy
 - This command will not merge changes from the remote into your local repository. It brings those changes onto what's called a remote branch. 
 - `git merge origin/master`:command to integrate origin/master into your local master branch.
 
We're ready to contribute some work. The workflow for Git collaborations typically follows this order:

  1.  Fetch and merge changes from the remote
  2.  Create a branch to work on a new project feature
  3.  Develop the feature on your branch and commit your work
  4.  Fetch and merge from the remote again (in case new commits were made while you were working)
  5.  Push your branch up to the remote for review
  
  >Steps 1 and 4 are a safeguard against merge conflicts, which occur when two branches contain file changes that cannot be merged with the git merge command.

Example

1. `cd clone-repo` : Go to clone repo folder
2. `git branch future` : Create new branch
3. `git checkout future` : Switch to your new branch
4. Do changes(adding, changing, deleting etc.) and `git add` and `git commit -m`

  Now it's time to share our work with remote. 

5. `git push origin your_branch_name`: git push origin future

    > output like that:To /home/ozgur/./yerel-depo/
    
    > *[new branch]      future -> future

6. Now goto main repo and merge the `future` branch
 - `git merge future` : 

Let's review.

    A remote is a Git repository that lives outside your Git project folder. Remotes can live on the web, on a shared network or even in a separate folder on your local computer.
    The Git Collaborative Workflow are steps that enable smooth project development when multiple collaborators are working on the same Git project.

We also learned the following commands

    1. git clone: Creates a local copy of a remote.
    2. git remote -v: Lists a Git project's remotes.
    3. git fetch: Fetches work from the remote into the local copy.
    4. git merge origin/master: Merges origin/master into your local branch.
    5. git push origin <branch_name>: Pushes a local branch to the origin remote.
    6. goto remote branch and merge <branch_name>: `git merge future`


# Step by Step Example for Local Teamwork

We want to make a Shopping List
- Mom has the `mom-repo`(this is the main repo) and she has all power :)
- Father will have the cloned `father-repo` and he has no power about this topic ;)
- They are working on same network on linux

# Let's begin
### mom is on computer and creating `mom-repo`

1. `git init mom-repo` : initialize mom-repo

 >`output`Başlatılan boş bir Git deposu, konum: /home/ozgur/mom-repo/.git/

2. `echo "1. Eggs" >> shopping_list.txt`: create shopping_list.txt with eggs :)
3. `git add shopping_list.txt`: git add
4. `git commit -m "Shopping list created"`: git commit -m ""

  `output`
 >[master (root-commit) e922536] Shopping list created
 
 >1 file changed, 1 insertion(+)
 
 >create mode 100644 shopping_list.txt

### father is on computer and cloning `mom-repo` as `father-repo`

1. `git clone /home/ozgur/mom-repo/ /home/ozgur/father-repo`: clonnig `mom-repo` as `father-repo` 

 >Don't forget this is my directory you must use your directory :)
 
2. `git branch future`: create "future" branch
3. `git checkout future`:choose "future" branch
4. `echo "2. Milk" >> shopping_list.txt`: Added "2. milk" to shopping_list.txt file
5. `git add shopping_list.txt`: git add
6. `git commit -m "Milk added"`: git commit -m
7. `git push origin future`: push future branch to origin(this is remote repo master branch)

### mom is again on computer and merge time:

1. `git branch`: control branch

> output is:

>future

>*master

2. `git merge future`: future merged to master 

 >That's all :)

3. `git log`: You can see what have you done in log file



You can find more example on: https://www.codecademy.com/learn/learn-git
