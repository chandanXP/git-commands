# Gitbash (windows):
> cd [folder path]

# To set username or email.
> git config --global user.name "Chandan"
> git config --global user.email "imjunior471@gmail.com"

# Will create gitignore file, certain files must be untracked.
> touch .gitignore 

# Initialize the git repository (empty).
> git init 

# Adding changes made to current directory.
> git add .

# Committing to the local repository.
> git commit -m "initial commit"

# Checking health of the repository.
> git status 

# Go to Github website click on "SSH" and copy the [link] from the newly created repository and then,
> git remote add origin [link]

# Upload local repository content to a remote repository.
> git push origin main
# OR
> git push origin master

# -----------------------------------------------------------
# NEW: HISTORY & RECOVERY (TIME TRAVEL)
# -----------------------------------------------------------

# View commit history (compact) to find the Commit Hash (e.g., 862bc71).
> git log --oneline

# Recover a SPECIFIC FILE from the past (saves it as a new file so you don't overwrite current work).
# Usage: git show [commit_hash]:[path/to/file] > [temp_file_name]
> git show 862bc71:client/src/lib/invoicePdf.ts > old_invoicePdf.ts

# Go back to a past state in a NEW BRANCH (Safe method to run/test old code).
# Usage: git checkout -b [new_branch_name] [commit_hash]
> git checkout -b old-code-review 862bc71

# Return to the latest code (if you switched branches or detached HEAD).
> git switch main
