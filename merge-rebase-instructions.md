###QUICK AND DIRTY

`git checkout your-branch-that-has-changes`

`git fetch citrondigital`

`git merge citrondigital/participants`

`git push origin your-branch-that-has-changes`

###PROPER WAY

`git checkout your-branch-that-has-changes`

`git fetch citrondigital`

`git rebase citrondigital/participants`

fix all the changes, follow the rebase instructions

`git add`

`git rebase --continue`

`git push origin your-branch-that-has-changes`
