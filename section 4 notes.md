git initialized in .git folder not current folder(kinda how git works)
learning-git-withbogdan/.git/

By default there are will be config, description, HEAD files, info, objects,
hooks, refs dirs
There are 4 kinds of objects in git. Blob, tree, commit, annotated tag.

Blob store all files, tree information about dirs, commit store different version
of our project,
annotated tag persistent text pointer to spesific commit

Git use sha1 hash function, hash function has 2 important features, first one, it
is one way(key word to has) function, secondly,
function will create the same hash based on the same input

when create object in git file, first 2 charachters is used to create folder,
the rest is used as a file name
