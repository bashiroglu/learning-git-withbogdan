Branch is text referance to commit

Branch poineter move after every commit and point last commit by default

in heads folder we can find braches(by default master)

Head is pointer to spesific commit or branch

we can change head by commanding git checkout branchname or commit hash

when we command git checkout we only change head file and git head which was 
pointing to master by default

detached Head means Head points to commit directly

preferably or by convension, head points branches not commits

git branch -list all local branches

git branch nameOfBranch -create new branch

git checkout nameOfBranch -checkout named branch

git checkout -d nameOfBranch(only merged) -delete named branch

git checkout -m currentNameOfBranch newNameOfBranch -rename branch

git checkout -b nameOfBranch -create named branch and checkout

when we create new branches, it points the same commit with master by default

even in new branches if the content of our newly added and commited file is the same with 
any file from other commited files, git doesn't create new blob object, just use the 
referance to previous file

