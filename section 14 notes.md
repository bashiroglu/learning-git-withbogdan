# Rebasing

Rebasing is kinda merging, but rebasing is also
It is all about making linear commit histoy, this can be beneficial sometimes, but also cause to lost history or to rewrite commits.

This process is two parts process. We cna explain it with 4 steps. first 2 one is about rebasing, let's imagine we have feature 1 branch and master branch. When we merge, our feature brach would merge to master but commits will stay in history of our commits (and last commit will have 2 parent commit ). But when we rebase, firstly we checkout feature branch `git checkout <name of feature branch>`, in there we run `git rebase master`, then 2 step start we checkout master `git checkout master` and merge `git merge <name of feature branch>`
That is by this series of actions, we will have brand new liner commit line, last ones are from feature branch.
