## Task 10 : Screenshots of bad commit and reverting it back

- git log after bad commit
![git log --oneline after bad commit](screenshots/log%20after%20deleting%20index.css%20file%20by%20mistake.png)

- git log after revert
![git log --oneline after revert](screenshots/After%20reverting%20the%20mistake.png)

## When to use git revert?    
- git revert does the exact opposite of what a commit does in order to go back, without wiping history.          
- git revert creates a new commit to go back, which means it keeps the branch's history intact so it is really helpful when working on remote or in a team of multiple developers leading to fewer conflicts.

## Task 10 : Screenshots of reset --hard and recovery using reflog
- git reset --hard
![git reset --hard](screenshots/git%20reset%20--hard.png)    

- git reflog
![git reflog](screenshots/git%20reflog.png)     

- recovery using git reflog
![recovery using git reflog](screenshots/recovery%20using%20git%20reflog.png)    

- fast forward merge from recovery branch
![fast forward merge from recovery branch](screenshots/fast%20forward%20merge%20from%20recovery%20branch.png)

## When to you use git reset --hard
- git reset --hard wipes out the history of one or a list of commits to undo the changes.
- One must be very careful whilst using git reset --hard as it rewrites the history, so undoing a git reset --hard is not an option.

## Never reset --hard on a remote repository or a repository on which other developers are working, because git reset --hard rewrites history and if some other developer is reliant on that specific commit it will lead to a ton of conflicts.