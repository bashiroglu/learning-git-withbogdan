we have 3 main area in git

1. working directory
2. staging area(index)
3. gti repo

git config --list - to see global git configuration username etc
git config --global user.email- to setup our details
git config --global user.name- to setup our details
git commit -m "our message" -setup commit message

[master *in first commit we will see here*(root-commit) (branch name)
d0c51c3*part of sha1 hash*]
added state managing funct. to login and sign up _our message_

commit points to tree object, inside of commit object there is pointer which point to tree hash
and in commit object we can see author(wrote changes) and commiter(commited changes)
and at the end we will see our commit message

root commit is kinda our first commit

git status -current status of git repo
-current branch
-if there are some changes to be commited
-changes related to files(will be showen)

git add - add files to staging area
-working dir to staging area

git commit -write changes to git repo
-create commit object
-this also can create blob if needed

git log -history of commits

gir checkout - checkout any commmit or branch
-to travel different versions of our project

git ls-files -s -to see files in git repo

in git there are 3 tracking statuses untracked, modified, staged, unmodified

by default status is untracked

modified, staged and unmodified are kinda tracked

we can use git add to track file

commit makes files unmodified, when we command git status and
the files which we don't get any information are unmodified

when we modified files they transition from unmodified to modified
and git status show them in different sections

we can use git add to stage area(staged)

we can also untack files, we may need this for example we we commited file by mistake

git add require an argument (argument which is supposed to be track)
(for example . says to track all listed files)

after git add we will see we transformed file to staged area, we can check it by command git ls-files

git rm --cached filename.ext -this unstage the file
in other words, this transform data fron stage are to working dir

6 files changed, 33 insertions(+)_it means 33 line added_, 15 deletions(-)_it means 15 line deleted_

after second commit, we will observe that we created new one commit object, one tree object and one blob object
in commit object we can see parent hash, it is hash of our previous commit, it is probably used to go back in
amoung our versions. tree hash is tree object hash of this commit, it is created newly, and it contains hashes of
files but the blob of files which we didn't changed will be still the same because content didn't change and no need
to create new blob for them but ones which of content changed, there will be new blobs. that is all

please also note that old tree will be still exist and will have its own structure, because it is important
for later to switch amoung commits

please not that in our first commit for project, we won't have parent commit and as a result hash neither
