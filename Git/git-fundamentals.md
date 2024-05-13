GIT

Git is a version control system.

Characteristics of Git:
* explicit;


Git Basics:
* git init – create a new git repository and begins tracking;
* git add – move modified files into the staging area;
* git status – shows you the status of your files;
* git commit – create a snapshot and commit to .git;
* git config – set and read specific Git configuration;
* git log – shows the committed snapshot history;
* git diff – shows changes between your working directory and staging areas;


Git Branches:
* git branch – list, create or delete branches;
* git checkout – switch between branches;
* git merge – bring changes from one branch into another;


Remote Repositories:
* git clone – copies an entire repo into a new local .git directory;
* git remote – create and show linked repositories;
* git push – send updates to associate repositories;
* git pull – retrieves and integrates changes from other repositories;
* git fetch – retrieves but doesn’t integrate changes from other repositories;

Undoing Changes:
* git revert – create a new commit that undoes a previous commit;
* git reset – remove files from the staging area;

* git <command> --help

Example:
* git add --help
* Git status
* code . = open editor VS Code


Example of adding and pushing a commit:
* Git add .
* git status
* git commit -m [name of commit]

Example of creating a new branch:
* git branch [name of branch]
* git branch -a = display branches in local repo
* git checkout [name of branch] = name of the branch we want to go to