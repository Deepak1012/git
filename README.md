# git_commands
Related to git commands

# Create new git folder in local 
git init()

# Add all files in local 
git add .

# Add particular file
git add file path

# Commit all files 
git commit -am"Message"

# Push to remote
git push 

# Pull from origin
git pull

# add upstream
git remote add upstream <url>
  
# sync local branch with remote
git fetch <remote_name>
git pull <remote_name> <branch_name>

# create new branch 
git checkout -b <branch_name>

# create new branch from remote upstream
git fetch upstream
git checkout -b <branch_name> upstream/<branch_name>

# Push branch to remote
git push <remote> <branch_name>
  
# Check commits in local
git log
git log --stat # for some abbreviated stats for each commit
git log --pretty=oneline
git log --pretty=format:"%h - %an, %ar : %s"
git log --pretty=format:"%h %s" --graph
git log --since=2.weeks

# remove commit from local and remote
git log --pretty=oneline --abbrev-commit
git rebase -i HEAD~<sr.no for commit>
git push <remote_name> <branch_name>


# Delete branch from local 
git branch -d <branch_name> # -d for --delete
git branch -D <branch_name> # -D for --delete --force

# Delete branch from remote
git push <remote_name> --delete <branch_name>
# or
git push <remote_name> :<branch_name>

