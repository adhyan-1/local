1. Local Repository Initialization and File Staging
Initialized a local Git repository using git init.
Created initial.txt and committed it to the main branch.
Created and staged temp.txt.
Practiced unstaging files using:
git restore --staged
git reset HEAD
Modified files, staged them again, and observed changes using git status.

2. Remote Repository Operations (GitHub)
Created a remote repository on GitHub.
Connected the local repository to GitHub using git remote add origin.
Pushed the initial commit to the remote main branch.
Modified files directly through GitHub's web interface.
Retrieved remote changes using git pull origin main.
Practiced staging multiple files and selectively unstaging one file.
Committed and pushed selected changes to GitHub.
Used git status to track repository states.

3. Branching and Pull Requests
Created a remote branch named g1 on GitHub.
Retrieved remote branch information using git fetch origin.
Checked out the g1 branch locally.
Created g1_file.txt, committed it, and pushed it to GitHub.
Created a Pull Request (PR) from g1 to main.
Successfully merged the PR without conflicts.

4. Local Git Operations and Reset Commands
Updated local branches using git fetch origin and git merge origin/main.
Created commits and practiced different reset operations:
git reset --soft HEAD~1 – Undo the last commit while preserving staged changes.
git reset --mixed HEAD – Unstage changes while preserving file modifications.
git reset --hard HEAD~1 – Remove the last commit and discard associated changes.
Used git add -p for interactive, selective staging.
Compared branches using git diff main g1.
Listed tracked files using git ls-files.
Inspected repository changes using git status and git log.

5. Local Branch Creation, Merging, and Conflict Resolution
Staged multiple changes across files.
Unstaged all changes using git reset --mixed HEAD.
Selectively staged changes using git add -p.
Examined staged changes using git diff --staged.
Compared differences between branches.
Merged branches in sequence:
b3 into b2
b2 into b1
b1 into main
Introduced a merge conflict by modifying the same line in initial.txt on two branches.
Manually resolved the conflict and completed the merge.
Deleted local branches using git branch -d.
Deleted the remote g1 branch using git push origin --delete g1.

6. Forking and Cross-Repository Collaboration
Forked your own GitHub repository into another repository under your account.
Cloned the forked repository locally.
Created a new file named forked.txt.
Committed and pushed changes to the forked repository.
Created a Pull Request from the forked repository to the original repository's main branch.

7. Advanced Staging, Stashing, and Conflict Resolution
Created a complex working scenario involving:
Modified initial.txt.
Modified b2_file.txt.
Created a new file challenge.txt.
Performed the following operations:
Staged all changes using git add ..
Unstaged challenge.txt using git reset HEAD challenge.txt.
Selectively staged lines using git add -p.
Committed selected changes.
Saved remaining changes using git stash.
Retrieved saved changes using git stash pop.
Handled and manually resolved a stash application conflict.
Committed the resolved changes.
Monitored repository states using git status and git diff.
Git Remove and Revert Operations
Practiced removing files using git rm.
Understood the difference between removing a tracked file from the working directory and removing it from Git tracking.
Practiced undoing committed changes using git revert.
Examined the effects of revert operations on commit history.
Verified file and repository states using git status, git diff, and git log.
