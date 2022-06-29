# Git Commands

|Command|Description|
|-|-|
|**Basic Commands**|
|git --version      |Check the version of git installed|
|git update-git-for-windows  |Update git for windows|
|git init    |Initialize the git in working directory|
|git status |Check working directory and staging area status|
|git ls-files |List files in staging area|
|git log |Display all commits of current branch in detailed view|
|git log --oneline |Display all commits of current branch in short view|
|git branch |Check current branch|
|**Commit Changes**|
|git add file1 file2|Add file changes to staging area|
|git add . |Add all changes to staging area|
|git commit -m "your_message" |Commit your changes in staging area|
|**Branch Creation and Deletion**|
|git branch branch_name |Create a new branch|
|git branch -d branch1 branch2|Delete branch if it is merged with any other branch|
|git branch -D branch_name|Force delete the branch|
|git checkout branch_name or git switch branch_name|Switch to specific branch|
|git checkout -b branch_name or git switch -c branch_name |Create and switch to new branch|
|git merge other_name |Bring other branch changes to current branch|
|**Detached Mode**|
|git checkout commit_id or git switch --detach commit_id |Switch to a specific commit in detached mode|
|git branch branch_name detached_mode_commit_id |Place detached mode changes in new branch to merge with others|
|**Undo Working Directory Changes**|
|git restore file_name or git restore . or git checkout file_name or git checkout .|Undo unstaged tracked file changes in WD. Changes will be removed.|
|git rm file_name |Remove file from staging area|
|git clean -dn |Show what are the newly created files will be deleted in WD|
|git clean -df |Force delete the new files in WD|
|**Undo Staged Changes**|
|git restore --staged file_name or git restore --staged . or git reset file_name or git reset .|Undo the changes from staging area, but changes wont be removed from WD|
|**Undo Commits**|
|git reset HEAD~1|Go back to previous commit and undo the changes from staging area|
|git reset --soft HEAD~1|Go back to previous commit and keep the changes in staging area|
|git reset --hard HEAD~1|Go back to previous commit and remove changes in WD|