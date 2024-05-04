<h1>This repository contains git information and git commands</h1>

git is a disctributed version control system(DVCS).</br>

Types of version control system</br>
1) Local Version Control System(VCS)</br>
It is like code available on devloper machine which is accessible to dev only.<br>
2) Centralized Version Control System(CVCS)</br>
It is have central repository where multiple can contribute/share code on central repository.</br>
3) Disctributed Version Control System(DVCS)</br>
It is like combination of local + centralise i.e developer have copy of code on their machine and also on central repository.</br>

<h3>History of Git</h3>
Previously open source contribution was done by sending binaries and patches, Linus Torvalds started git in 2005 as bitkeeper stated charging.
Previously default branch in git was master later it named to main.

<h3>Differnt Areas of Git</h3>
Local repo => Working Directory => Staging Area => commit Hostory => git => push => remote repositiry

<h3>Configure git</h3>

|git config --global --list    |list git configuration|
|------------------------------|----------------------|
|git config --global user.name |set username          |
|git config --global user.email|set email             |

<h3>Getting & Creating Projects</h3>

|git init    |Initialize a local Git repository|
|------------------------------|----------------------|
|git init -b main |create local git branch named main if not specify then master default|

<h3>Basic Snapshotting commands<h3>

|git status | check status|
|------------------------------|----------------------|
|git add fileName.txt |to add into staging area|
|git add .|to add all files present in current branch in staging area|
|git commit -m "commit message"| to commit |
|git rm -r fileName.txt| detele file|
|git rm --cached fileName.txt | unstage file from .git|
|git commit -a -m "commit message" | commiting without adding into staging area|

<h3>Inspection & Comparision</h3>

|git log | view changes |
|--------------|------------|
|git log --summary | view changes(detailed)|
|git log --online | view chnages(briefly)|
|git log --graph | graph view |
|git diff (sourse branch) (target branch) | preview changes before merging|
|git diff | diff between modify and previous commit|
|git diff --staged | diff with last commit & staged change | 

<h3>Branching & Merging</h3>

|Command |	Description|
|------------|--------------|
|git branch|	List branches (the asterisk denotes the current branch)|
|git branch -a|	List all branches (local and remote)|
|git branch [branch name]|	Create a new branch|
|git branch -d [branch name]|	Delete a branch|
|git checkout -b [branch name]|	Create a new branch and switch to it|
|git checkout -b [branch name] |origin/[branch name]	Clone a remote branch and switch to it|
|git branch -m [old branch name] [new branch name]	|Rename a local branch|
|git checkout [branch name]	|Switch to a branch|
|git checkout -	|Switch to the branch last checked out|
|git checkout -- [file-name.txt]	|Discard changes to a file|
|git switch [branch-name]	|Switch to branch|
|git switch -c [branch-name]	|Create new branch |
|git branch -m [branch-name]	|Create new branch |
|git merge [branch name]	|Merge a branch into the active branch |
|git merge [source branch] [target branch]	|Merge a branch into a target branch |

