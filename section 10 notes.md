#Git push, fetch and pull

When we change some file, this doesn't reflect in remote repo. 
In order to reflect it, we have to add stage area, commit and push to remote repo.

When someone pushed ro remote repo and we want those changes in our local repo, 
we are supposed to pull or fetch that repo. 

Fetch basically bring the branches from remote repo. 

Git pull consist  of 2 parts, it firstly fetch then merge.

Origin is default name of remote repo.

git remote - list all remote services 

git remote -v -list links to push and to fetch(pull)

git branch -list only local branches

git branch -a - list all branches(including remote ones)

git branch -r - list only remote branches

git branch -vv  list tracking branches(means branch has its branch in 
remote(when we commit and push it will push respectively))

when we create(by commanding git checkout NameOfRemoteBranch)
branch in local repo with the same name in remote, it will automatically
will be tracking branch of remote branch. 

git remote show origin -additional information about remote branch

git fetch only update single checkout branch, not others

when we pull, git create FETCH_HEAD file which is basically
contains names and last commits of remote branches and the ones which is not 
checkouted while commanding, will include "not-for-merge"

git pull -v -pulling by observing process of pulling

merge which happens while pulling is the same with normal merge, again there is 2 options 
3 ways and fast-forward

When we merge pull from remote, we can face conflicts, resolution of conflicts is the same. 

Remember that after pulling, we have push to reflect what we have locally. 







