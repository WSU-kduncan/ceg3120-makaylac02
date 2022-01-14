 Git Guide - Makayla Carr

## Command line git

- status
  - Shows status of the local repository. This status includes:
    - number of local commits that have not been synced with remote (GitHub)
    - list of files in local folder than are NOT being tracked by git
    - list of files in local folder that have changes that need to be committed
  - `git status`
- clone
  - Creates a copy of the target repository
  - `git clone (link)`
- add
  - Adds files for tracking by git.
  - `git add filename`
- rm
  - Removes tracked files in git
  - `git rm filename`
- commit
  - Commits any changes to a file. Creates a changelog
    - where you can keep track of updates. This commits
    - any files that have been added using git add.
  - `git commit`
- push
  - Pushes any commits made to Github. Brings things up to date.
  - `git push`
- fetch
  - Downloads content from other repositories. 
  - `git fetch <repository> 
- merge
  - Merges two branches together. 
  - `git merge name`
- pull
 - Adds changes from another repository into the current branch
   - and updates the branch if it is behind
 - `git pull <repository>
- branch
  - Lists, creates, or deletes branches
  - `git branch'
     - `-d` = deletes, `move` = moves, - `-l` = lists, 
- checkout
  - Switches branches 
  - `git checkout` <branch>
- ~~init~~
- ~~remote~~

## git files & folders

- .git folder
  - Holds all information on commits and project history
- .gitignore file
  - Specifies intentionally untracked files to ignore 
  - `gitignore filename`
- ~~.git/hooks~~

## GitHub

- Pull requests
  - Requests for code to be reviewed so that they 
    - can verify if they are ready to merge
- SSH authentication to repositories
  - Public ssh key on local system is put into github settings 
- ~~Actions~~

