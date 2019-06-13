# Configure git
!git config --global user.name 'First Last'
!git config --global user.email 'name@domain.com'
!git init

# Ignore File

.gitignore is a hidden file in the top-level folder used to specifiy specific files and folders or patterns that should be ignored by our repository. Typically things like images and data should not be kept in version control due to their large size. One other folder or file that is excluded are configuration files as they may contain sensitive information or passwords that can become public if kept in a repository. Check out [this article](https://damnhandy.com/2015/09/10/how-putting-credentials-in-git-can-cost-you-at-least-6500-in-just-a-few-hours/comment-page-1/) for an example of where commiting an amazon web services crediential to github racked up $6,500 worth of charges when someone used their now public credientials.

# View status and log
!git status
!git log

# Add or remove from staging area
!git add [target]
!git reset [target file or commit]
!git reset --hard origin/master

# Automatically stage tracked files, 
# including deleting the previously tracked files
# Does not add untracked files
!git add -u

# Delete files and stage them
!git rm [target]

# Commit
!git commit -m “Add commit message here”

# Add new origin
!git remote add origin https://github.com/donnemartin/ipython-data-notebooks.git

# Set to new origin
!git remote set-url origin https://github.com/donnemartin/pydatasnippets.git
    
# Push to master, -u saves config so you can just do "git push" afterwards
!git push -u origin master
!git push

# Diff files
!git diff HEAD
!git diff --staged
!git diff --cached

# Show log message of commit and diff
!git show $COMMIT

# Undo a file that has not been added
!git checkout — [target]

# Revert a commit
!git revert

# Undo a push and leave local repo intact
!git push -f origin HEAD^:master

# Undo commit but leave files and index
!git reset --soft HEAD~1

# Amend commit message of most recent change
!git commit --amend
!git push --force [branch]

# Create a branch
!git branch [branch]

# Check branches
!git branch

# Switch branches
!git checkout [branch]

# Merge branch to master
!git merge [branch]

# Delete branch
!git branch -d [branch]

# Clone
!git clone git@github.com:repo folder-name
!git clone https://donnemartin@bitbucket.org/donnemartin/tutorial.git
    
# Update a local repository with changes from a remote repository
# (pull down from master)
!git pull origin master

# Configuring a remote for a fork
!git remote add upstream [target]

# Set remote upstream
git branch --set-upstream-to origin/branch

# Check remotes
!git remote -v

