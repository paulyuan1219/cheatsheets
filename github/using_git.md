# Cheat Sheet in a Table
|                 Chapter                  |                  Command                  |                                  Command with options and arguments                                   |                                                                                                                                                                                                                                                                                                    Explanation                                                                                                                                                                                                                                                                                                    |     |
| :--------------------------------------: | :---------------------------------------: | :---------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | --- |
|       1. Git and the Command Line        |                git config                 |                                      git config --global --list                                       |                                                                                                                                                                                                                                                                                              List global config info                                                                                                                                                                                                                                                                                              |     |
|                                          |                                           |      git config --global user.name "wei yuan"<br>git config --global user.email "xxx@gmail.com"       |                                                                                                                                                                                                                                                                                             Set up global config info                                                                                                                                                                                                                                                                                             |     |
|          2. Local Repositories           |                 git init                  |                                               git init                                                |                                                                                                                                                                                                                                                                                          Initialize a Git repo under pwd                                                                                                                                                                                                                                                                                          |     |
|                                          |                                           |                                       git init -b <branch_name>                                       |                                                                                                                                                                                                                                                                                      Init a repo and set the initial branch                                                                                                                                                                                                                                                                                       |     |
|            3. Making a Commit            |                git status                 |                                              git status                                               |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |     |
|                                          |                  git add                  | git add <filename><br>git add <filename1> <filename2><br>git add -A # add all files under working dir |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |     |
|                                          |                git commit                 |                                   git commit -m “this is an update”                                   |                                                                                                                                                                                                                                                                                        Create a new commit with a message                                                                                                                                                                                                                                                                                         |     |
|                                          |                  git log                  |                                                git log                                                |                                                                                                                                                                                                                                                                                     Show commits for one branch in local repo                                                                                                                                                                                                                                                                                     |     |
|                                          |                                           |                                             git log —all                                              |                                                                                                                                                                                                                                                                                    Show commits for all branches in local repo                                                                                                                                                                                                                                                                                    |     |
|               4. Branches                | # A branch is just a pointer to a commit. |                                                                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |     |
|                                          |                git branch                 |                                              git branch                                               |                                                                                                                                                                                                                                                                                                List local branches                                                                                                                                                                                                                                                                                                |     |
|                                          |                                           |                                     git branch <new_branch_name>                                      |                                                                                                                                                                                                                                                                                                  Create a branch                                                                                                                                                                                                                                                                                                  |     |
|                                          |                                           |                                            git branch —all                                            |                                                                                                                                                                                                                                                                                 List local branches and remote-tracking branches                                                                                                                                                                                                                                                                                  |     |
|                                          |                                           |                                      git branch -d <branch_name>                                      |                                                                                                                                                                                                                                                                                               delete a local branch                                                                                                                                                                                                                                                                                               |     |
|                                          |                                           |                                            git branch -vv                                             |                                                                                                                                                                                                                                                                                  List local branches and their upstream branches                                                                                                                                                                                                                                                                                  |     |
|                                          |                git switch                 |                                       git switch <branch_name>                                        |                                                                                                                                                  Switch to a branch. Three steps involved.<br>1. <br>HEAD now points to the target branch.<br>2. Commit files —> Staging area files<br>3. Staging area files —> Working dir<br>Note: if a remote-tracking branch like <br>origin/feature exists, then git switch feature will create a new local branch feature.                                                                                                                                                  |     |
|                                          |                                           |                                      git switch -c <branch_name>                                      |                                                                                                                                                                                                                                                                                        Create and switch onto a new branch                                                                                                                                                                                                                                                                                        |     |
|                                          |               git checkout                |                                      git checkout <branch_name>                                       |                                                                                                                                                                                                                                                                                         Switch to a branch. Same as above                                                                                                                                                                                                                                                                                         |     |
|                                          |                                           |                                     git checkout -b <branch_name>                                     |                                                                                                                                                                                                                                                                                        Create and switch onto a new branch                                                                                                                                                                                                                                                                                        |     |
|                                          |                                           |                                       git checkout commit_hash                                        |                                                                                                                                                                                                                                                             Check out a commit. HEAD now points to a commit directly. This is a detached HEAD state.                                                                                                                                                                                                                                                              |     |
|                5. Merging                |                 git merge                 |                                        git merge <branch_name>                                        |                                                                                                                                                                                                                                                                       Step 1: switch to main<br>Setp 2: integrate <br>branch_name into main                                                                                                                                                                                                                                                                       |     |
|  6. Hosting Services and Authentication  |                                           |                                                                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |     |
| 7. Creating and Pushing to a Remote Repo |          # Based on a local repo          |                                  # On github, create rainbow-remote                                   |                                                                                                                                                                                                                                                                                              # stored in .git/config                                                                                                                                                                                                                                                                                              |     |
|                                          |                git remote                 |                                   git remote add <shortname> <URL>                                    |                                                                                                                                                                                                                                                                                    for local repo, add a connection to remote                                                                                                                                                                                                                                                                                     |     |
|                                          |                                           |                                              git remote                                               |                                                                                                                                                                                                                                                                           List the remote repo connections stored in local by shortname                                                                                                                                                                                                                                                                           |     |
|                                          |                                           |                                             git remove -v                                             |                                                                                                                                                                                                                                                                                             same as above, plus URLs                                                                                                                                                                                                                                                                                              |     |
|                                          |                 git push                  |                                  git push <shortname> <branch_name>                                   |                                                                                                                                                                                         Upload content from local <branch_name> to the <shortname> remote repo.<br>Two things happen:<br>1. A remote branch will be created in remote repo<br>2. A remote-tracking branch is created locally. See <br>.git/refs/remotes/*                                                                                                                                                                                         |     |
|         8. Cloning and Fetching          |                 git clone                 |                                   git clone <URL> <directory_name>                                    | Clone a remote repo. default is the same dir name. In detail:<br>1. create a project dir under pwd<br>2. create (init) the local repo<br>3. download all the data from remote repo.<br>4. Add a connection to the remote repo; by default the short name is <br>origin<br>After cloning, Git needs to know which branch it should be on. The <br>origin/HEAD pointer determines it.<br>Especially, <br>git clone will create remote-tracking branches for all the branches currently present in the remote repo being cloned, but the only local branch that is created is the branch that origin/HEAD points to. |     |
|                                          |                 git push                  |                                 git push <shortname> -d <branch_name>                                 |                                                                                                                                                                                                                                                                               delete a remote branch and its remote-tracking branch                                                                                                                                                                                                                                                                               |     |
|                                          |                git branch                 |                                            git branch -vv                                             |                                                                                                                                                                                                                                                                                  List local branches and their upstream branches                                                                                                                                                                                                                                                                                  |     |
|                                          |                 git fetch                 |                                         git fetch <shortname>                                         |                                                                                                                                                   download data from <shortname>. This command downloads all the necessary commits to update all the remote-tracking branches in the local repo to reflect the state of the remote branches in the remote repo that is specified.<br>**<br>It only affects remote-tracking branches, but not local branches.**                                                                                                                                                    |     |
|                                          |                                           |                                             git fetch -p                                              |                                                                                                                                                                                                                                                 Delete any remote-tracking branches that correspond to remote branches that have been deleted in the remote repo                                                                                                                                                                                                                                                  |     |
|           9. Three-Way Merges            |                git branch                 |                   git branch -u <shortname>/<branch_name><br>friend: git branch -vv                   |                                                                                                                                                                                                                                                                                Define an upstream branch for current local branch                                                                                                                                                                                                                                                                                 |     |
|                                          |                 git merge                 |                            git fetch && git merge origin/main && git push                             |                                                                                                                                                                                                                                                                          execute the three-way merge on local main branch, then push it.                                                                                                                                                                                                                                                                          |     |
|                                          |                 git pull                  |                                               git pull                                                |                                                                                                                                                                                                                                               If an upstream branch is defined for the current branch, fetch and integrate changes from the defined upstream branch                                                                                                                                                                                                                                               |     |
|                                          |                                           |                                git pull <shortname> <branch_name><br>                                 |                                                                                                                                                                                                                                                        Fetch and integrate changes from the <shortname> remote repository for the specified <branch_name>                                                                                                                                                                                                                                                         |     |
|           10. Merge Conflicts            |                 git merge                 |                                           git merge —abort                                            |                                                                                                                                                                                                                                                                         Stop the merge process and go back to the state before the merge.                                                                                                                                                                                                                                                                         |     |
|               11. Rebasing               |                git rebase                 |                                        git rebase <banch_name>                                        |                                                                                                                                                                                                                                                 Reapply commits on top of another branch. 假设从branch_name的commit开始，把当前branch上的变化一个个重新应用一遍。                                                                                                                                                                                                                                                 |     |
|                                          |                                           |                                         git rebase —continue                                          |                                                                                                                                                                                                                                                       continue the rebase process after having resolved merge conflicts, i.e. after running (git add file)                                                                                                                                                                                                                                                        |     |
|                                          |                                           |                                           git rebase —abort                                           |                                                                                                                                                                                                                                                                                 Stop rebase process and go back to previous state                                                                                                                                                                                                                                                                                 |     |
|                                          |                git restore                |                                    git restore —staged <filename>                                     |                                                                                                                                                                                                                                               Restore a file to another version of the file in the staging area. Only change a file’s version in the staging area.                                                                                                                                                                                                                                                |     |
|    12. Pull Requests (Merge Requests)    |                 git push                  |                     git push —set-upstream origin topic<br>friend: git branch -vv                     |                                                                                                                                                                                                                                                                                     set up a specific remote branch and push                                                                                                                                                                                                                                                                                      |     |
|                                          |                 git pull                  |                          git pull -p<br>friend: git branch -d <branch_name>                           |                                                                                                                                                                                                                                                 delete any remote-tracking branches that correspond to remote branches that have been deleted in the remote repo                                                                                                                                                                                                                                                  |     |
|                                          |                                           |                                                                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |     |
|                                          |                                           |                                                                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |     |
|              Miscellaneous               |               git cat-file                |                                      git cat-file -p <commit_id>                                      |                                                                                                                                                                                                                                                                                                 Inspect a commit                                                                                                                                                                                                                                                                                                  |     |


# Pushing commits to a remote repository
## `git push`
Use `git push` to push commits made on your local branch to a remote repository.

- `git push`: sends all matching branches that have the same names as remote branches.
- `git push REMOTE-NAME BRANCH-NAME`: you usually run `git push origin main` to push your local changes to your online repository.
- `git push REMOTE-NAME LOCAL-BRANCH-NAME:REMOTE-BRANCH-NAME`: Renaming branches
- `git push REMOTE-NAME TAG-NAME`: push a single tag
- `git push REMOTE-NAME --tags`: push all your tags
- `git push REMOTE-NAME :BRANCH-NAME`: delet a remote branch or tag. Resemble the same steps in Renaming branches.

## `git remote`
When you clone a repository you own, you provide it with a remote URL that tells Git where to fetch and push updates. If you want to collaborate with the original repository, you'd add a new remote URL, typically called `upstream`, to your local Git clone:

```
git remote add upstream THEIR_REMOTE_URL
```

Now, you can fetch updates and branches from their fork:

```
git fetch upstream
# Grab the upstream remote's branches
> remote: Counting objects: 75, done.
> remote: Compressing objects: 100% (53/53), done.
> remote: Total 62 (delta 27), reused 44 (delta 9)
> Unpacking objects: 100% (62/62), done.
> From https://github.com/OCTOCAT/REPO
>  * [new branch]      main     -> upstream/main
```
When you're done making local changes, you can push your local branch to GitHub and initiate a pull request.

# Getting changes from a remote repository

Options for getting changes
- `clone` and `fetch` download remote code from a repository's remote URL to your local computer
- `merge` is used to merge different people's work together with yours
- `pull` is a combination of `fetch` and `merge`.

## Cloning a repository

```
$ git clone https://github.com/USERNAME/REPOSITORY.git
# Clones a repository to your computer
```

When you run `git clone`, the following actions occur:

- A new folder called `repo` is made
- It is initialized as a Git repository
- A remote named `origin` is created, pointing to the URL you cloned from
- All of the repository's files and commits are downloaded there
- The default branch is checked out

For every branch `foo` in the remote repository, a corresponding remote-tracking branch `refs/remotes/origin/foo` is created in your local repository. You can usually abbreviate such remote-tracking branch names to `origin/foo`.

## Fetching changes from a remote repository
Fetching from a repository grabs all the new remote-tracking branches and tags **without** merging those changes into your own branches.

## Merging changes into your local branch
Typically, you'd merge a remote-tracking branch (i.e., a branch fetched from a remote repository) with your local branch:

```
$ git merge REMOTE-NAME/BRANCH-NAME
# Merges updates made online with your local work
```

## Pulling changes from a remote repository
`git pull` is a convenient shortcut for completing both `git fetch` and `git merge` in the same command:


```
$ git pull REMOTE-NAME BRANCH-NAME
# Grabs online updates and merges them with your local work
```

## Dealing with non-fast-forward errors
Sometimes, Git can't make your change to a remote repository without losing commits. When this happens, your push is refused.

If another person has pushed to the same branch as you, Git won't be able to push your changes:

```
$ git push origin main
> To https://github.com/USERNAME/REPOSITORY.git
>  ! [rejected]        main -> main (non-fast-forward)
> error: failed to push some refs to 'https://github.com/USERNAME/REPOSITORY.git'
> To prevent you from losing history, non-fast-forward updates were rejected
> Merge the remote changes (e.g. 'git pull') before pushing again.  See the
> 'Note about fast-forwards' section of 'git push --help' for details.
```

You can fix this by fetching and merging the changes made on the remote branch with the changes that you have made locally:

1. `$ git fetch origin`
  - Contacts the remote repository referenced by origin.
  - Downloads objects and refs (branches, tags, etc.) from the remote repository that do not exist in your local repository.
  - Updates your local references (such as remote-tracking branches) to reflect the state of the remote repository.
3. `$ git merge origin YOUR_BRANCH_NAME` : 
  - tells Git to merge the changes from a branch named YOUR_BRANCH_NAME on the remote repository (origin) into the branch you're currently on in your local repository. 
  - This is useful for updating your local branch with changes made in the remote repository or integrating work done in parallel by collaborators into your branch.


Or, you can simply use `git pull` to perform both commands at once:
```
$ git pull origin YOUR_BRANCH_NAME
# Grabs online updates and merges them with your local work
```

## Splitting a subfolder out into a new repository
You can turn a folder within a Git repository into a brand new repository.

暂时用不到，以后再看。

## About Git subtree merges
If you need to manage multiple projects within a single repository, you can use a subtree merge to handle all the references.

暂时用不到，以后再看。


## About Git rebase
The git rebase command allows you to easily change a series of commits, modifying the history of your repository. You can reorder, edit, or squash commits together.

Assume the following history exists and the current branch is "topic":

```
          A---B---C topic
         /
    D---E---F---G master
```

From this point, the result of either of the following commands:

```
git rebase master
git rebase master topic # === git checkout topic && git rebase master
```

would be:

```
                  A'--B'--C' topic
                 /
    D---E---F---G master
```


## Using Git rebase on the command line
Here's a short tutorial on using git rebase on the command line.

# About Git
## Example: Contribute to an existing repository

```
# download a repository on GitHub to our machine
# Replace `owner/repo` with the owner and name of the repository to clone
git clone https://github.com/owner/repo.git

# change into the `repo` directory
cd repo

# create a new branch to store any new changes
git branch my-branch

# switch to that branch (line of development)
git checkout my-branch

# make changes, for example, edit `file1.md` and `file2.md` using the text editor

# stage the changed files
git add file1.md file2.md

# take a snapshot of the staging area (anything that's been added)
git commit -m "my snapshot"

# push changes to github
git push --set-upstream origin my-branch
```

## Example: Start a new repository and publish it to GitHub
First, you will need to create a new repository on GitHub. For more information, see "Hello World." Do not initialize the repository with a README, .gitignore or License file. This empty repository will await your code.

```
# create a new directory, and initialize it with git-specific functions
git init my-repo

# change into the `my-repo` directory
cd my-repo

# create the first file in the project
touch README.md

# git isn't aware of the file, stage it
git add README.md

# take a snapshot of the staging area
git commit -m "add README to initial commit"

# provide the path for the repository you created on github
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY-NAME.git

# push changes to github
git push --set-upstream origin main
```

## Example: contribute to an existing branch on GitHub
This example assumes that you already have a project called repo on the machine and that a new branch has been pushed to GitHub since the last time changes were made locally.

```
# change into the `repo` directory
cd repo

# update all remote tracking branches, and the currently checked out branch
git pull

# change into the existing branch called `feature-a`
git checkout feature-a

# make changes, for example, edit `file1.md` using the text editor

# stage the changed file
git add file1.md

# take a snapshot of the staging area
git commit -m "edit file1"

# push changes to github
git push
```

