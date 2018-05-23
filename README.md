# Useful functions in git 

To clone a repository in github we want to take the URL of the repository and to then use the 

git clone name_of_repository 

This will download the repository locally to your machine. Then to make changes to the repository, we want to make a new branch. We do this by using the following code. 

git branch edit/name_of_change

We'll now have created another branch. We can check this by running 

git branch

This will show the branches that exist. To move into the new branch, we'll run 

git checkout edit/name_of_change

And then we'll start to do our work on the branch and then save the branch. Then if we run 

git status 

We'll be able to see the files that have changed. To put this branch into github, we'll then stage the files using 

git add .

Then we'll add a message to our future selves about what the changes were

git commit -m "I changed the readme file to give useful information"

Then we'll push our branch to github 

git push 

What if our local branches become out of sync with the master? We'll stash away our changes to the current branch we're working on using 

git stash 

Then we'll then use 

git pull 

Which will bring our old master branch in line with the new one, and not affect our changes

git checkout master

Then we'll go back to our main branch using 

git checkout edit/name_of_change

Then we'll then merge in our updated master branch to the changed branch 

git merge master

Then we'll re-add in our previous changes that we stashed away earlier

git stash pop

git status

Now we can see the branch is up to date and has the changes we wanted in our current branch! 






