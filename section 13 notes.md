# Git Tags

Git tags are kinda special names for branches. Difference from branches names is that tag names don't move while branche names are moving. Tags are mostly used for versions of website, they are created before releases(merging to master).

When we talk about git tags, we need to talk about CI & CD too.

Continuous integration and Continuous delivery(continuous deployment).
In this principle, software develop continuously. There are 2 environments in this kinda development. Staging and Production. Staging is for testing and developing the software but Production env is for clients only, and merging in that env is only allow a few people and after many tests, because of these reasons only a few merging is seen in a month.

Semantic versioning is method to name software versions.
v 1.0.2 1(major release) 0 (minor release) 2 (patch release)

There are 2 types of tags, annotated tag is tag with author name and date, lightweight text is without author name and date.

Lightweight tag files simply point to commit and they are not pushed to remote by default.
We can create lightweight tags by commanding
`git tag <tagname>`
We can create annotated tags by commanding
`git tag -a <tagname> -m "tag message"`

`git tag` to list tag names

`git tag -v <tagname>` details for tag name

after pushing our files to remote we can run
`git push -v --tags` to push tags to remote

`git push -v origin <tagname>` to push spesific tag name

We can also create tags and add messages in remote by using github. We can also pull those tags to local dir.
`git pull -v `