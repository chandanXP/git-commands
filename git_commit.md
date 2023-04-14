# Gitbash (windows):
> cd + [folder path]
# To set username or email.
> git config --global user.name "Chandan"
> git config --global user.email "imjunior471@gmail.com"

# Will create gitignore file, certain files must be untracked.
> touch .gitignore 

# Initialize the git repository(empty).
> git init 

# Adding changes made to current directory.
> git add .

# pushing to the remote repository.
> git commit -m "initial commit"

# checking health of the repository.
> git status 

# Go to Github website click on "SSH" and copy the [link] from the newly created repository and then,
> git remote add origin [link]
# + [Enter key]

# Upload local repository content to a remote repository.
> git push origin main
> git push origin master