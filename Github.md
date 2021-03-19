### To move one Github repository into another

First create local copy of repository
`git clone repository.git`
Then `cd` into this new repository
`cd repository-name`
Copy the repository you want to move into the new repository
`git submodule add repository-to-be-added.git`
Add and commit message
`git add .`
`git commit -m 'message'`
Then push to the destination repository
`git push destination-repository`

## To make changes to a submodule after it's added to a repository

First cd into the submodule folder
`cd submodule-folder`
Then add files that have been changed
`git add .`
`git commit -m 'commit message'`
Get into the parent folder
`cd ..`
Add and commit again
`git add submodule-folder`
`git commit -m 'commit message'`
Push changes
`git push destination-repository`
