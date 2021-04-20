# What is Git?
   Git is version control system that allows for collaborative projects to be worked on in real time with changes maintained and clearly communicated, with the ability to revert to previous versions as needed.
### Without Version control:
   - multiple variations of the same file
   - files keep building up 
   - changes are difficult to follow
### GitHub Snapshots
   - each commit saves a new version
   - changes are easy to follow and recorded
   - all info stored in one file
### Keeping Track
   - Each commit has a corresponding label
   - HEAD = most recent version
   - Messages on commits can explain changes
   - Clear effective commit messages are critical on large projects
   - maintain professionalism and label each commit
## GitHub
   - primary cloud for code storage and collaboration
   - easy backups for code via cloud storage
   - allows changes to be made separately until ready for combining

## Putting it all Together
   - With proper GitFlow, teams can easily work together
   - File history is easy to access

# What is a Repository?
   - A set of files or an entire project that Git is to pay attention to 
   - Usually one repository per project
   - Repositories can live both locally and on the cloud

# Syncing a file with GitHub
   - all assignments must be public, private code cannot be deployed
   - command 'git clone {link}' makes the terminal download the repo and connect it as a Git file
   - both copies are sync'd. 
   - now you can open a text editor within the file to begin working on the git file while sync'd with the cloud copy

## ACP (Add, Commit, Push)
   - When a change is made, git stages the changes with (A)dd
   - (C)ommit means changes are ready to push
   - (P)ush sends the updates to GitHub
   - 'git add filename' stages changes 'git add .'
   - 'git commit -m "message"' allows you to commit with message
   - 'git push origin main' sends the updates to the main branch of the origin
   - each step must precede the next, or the process will fail
   - it is helpful to run 'git status' between each step to verify status
   - changes can be stored away for later use via 'git stash' and retrieved with 'git stash apply'
