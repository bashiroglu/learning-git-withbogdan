we have 2 kinda merging 1. fast-forward merge 2. 3 ways merge

in every merge we need to 
1. create new branch 
2. change files and commit changes
3. checkout main branch 
4. command merge process by -git merge feature-branchName 

Please remember that Git itself will decide which way to use depends on whether you have
new commits in you branch or not

1. fast-forward merge: this is possible when we don't have new commits 
after creating new branch in master branch. And in this case, we are supposed to be
in master(HEAD> Master) we simply change master and Head to last commit of new Branch

2. in 3 way merge, we have 3 main point 
1 one is ancestor: where both branch have common commit, 
2 master branch(receiver) and the feature branch. In order to merge
we need to switch back to master and there we need to command for merge,
command merge (git merge nameOfFeatureBranch), in this kind of merging our merged commit will have 

2 parent commit, we may delete feature branch but commits will always be there for history.

above notes was about 3 way merge without conflict. 

Conflicts happens when we have changed line in both our branches, in that case git ask us(after merge command) to
resolve manually(going to editor or nano command interface and delete or change conflicted lines)
conflicts then to add and commit 
