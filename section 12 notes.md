# Forks and contribution to the public repositories


We can fork any public repo and when we fork we own the same repo files (files were exist when we fork). But that new our own repo won't have any connection with its parent(where we forked) repo. In order to have connection, we have to explicitily make connection. For that we can another remote server(when we create we will have only one origin (point to our remote repo))

```bash
git remote add upstream(name of new remote server) link of forked repo
```


we made connection but we don't have files(new files, the files which are added after we fork) yet.

in order to get files, we are supposed to pull the files (changed files) from forked repo

```bash
git pull upstream master
```

Remeber when we pull we actaully fetch, then merge. We got our files but our own repo is still unupdated, in order to update it, we have to push our files there

```bash
git push
```



