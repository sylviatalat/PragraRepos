***** DevOps class April 14 summary from a student understanding ******

Git

# Create a repository in GitHub (Remote)
# Once Repos is created, copy the ssh link of that Repos (or use clone tab if provided) 
# Paste the link in your local Terminal (git-bash) by using this command:
 git clone -paste link-
 git init

# You should see the name of the repos that you created and brought to local Terminal, on the left panel
# Right click on the name of that Repos and creat a file call it README.md

 cd to the newly created Repos
 git add README.md (or git add .)
 git status   
       you should see README.md in green color (means you are in staging area)

# Add content to the README.md file (your code)
 git commit -m "New changes" 
 git status
       you will see white color messages. your code is now in the local repository

 git push --set-upstream origin main 
      to set the remote repository as upstream (setting up the infrastructre where you code should reside in the remote repo)

      go back to github and you should see the README.md there with the content


Branch
Git branches are effectively a pointer to a snapshot of your changes.

# To create a branch :               
 git branch branch_name 
# To check the list of branches:     
git branch
The branch that you are currently on is listed in green with an *

# This branch is only created in your local machine; use the following command to push this branch to your central Repository(Remote)
 git push --set-upstream origin branch-name

# To switch to between branches use this command: 
 git checkout branch_name     -or
 git switch branch_name

# check to see if you are in the correct branch: 
  git branch 

# To delete a branch: 
git branch -d branch_name

