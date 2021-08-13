to alter any commit message
that is to re write anu previous commit message
refer
https://stackoverflow.com/questions/179123/how-to-modify-existing-unpushed-commit-messages


git commit --amend -o -m "New commit message"
this will only change the last commit message
--------------------------------------------------------------
If it's a buried commit, use the below rebase comment 

git log --oneline 
    7ddd213 commit 1
    5tt8047 commit 2
lets say you have to change the second commit (commit 2)

git rebase -i @~2   (# Show the last 9 commits in a text editor)
Find the commit you want to change 
then  change its  pick to r (reword), and save and close the file.(esc , :wq) 
then it will open a new window
where you can change that particular commit message
press i at first to enter in to insert(edit) mode


i--> to enter insert mode — text you type will appear in the file
