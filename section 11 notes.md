# Git Pull requests

Git is also collaboration service for developers. Developers can own repo and collaborate in that 
repo with others. In order to be accepted offered changes, owner or several(this is choice of owner)
developers. 

They use communication method called Pull request(in some VCS merge request) when a developer 
want to change something create branch and after finished his or her job, developer can pull 
request (it is kinda saying, I finished please review and if okay, accept). 

This can be both in repo (in this kind of cases merge request make more sense) and forked repo
(in this case pull request may make more sense because he cannot directly request merge)

Developers can review changes both locally and globally. 

git config --list -show settings(details) of git config file 

git config amend --author="Name of Githubber<Email of Githubber>"

After commits, let's say we want to push our local commits of particular Branch to Github
but we don't have upstream branch of particular Branch, that is why we need to set firstly 
by commanding "git --set-upstream  <Name of Branch> <Name Of Origin>" (--set-upstream = -u)
(git push --set-upstream origin useritem)

after creating the remote upstream branch, we get link in command line and we can create new 
pull request by going that link. 

By using Github interface we can compare, create new pull request and review.

Please remember that, it is convention to add name of branch in the beginning of pull request name.

After pull request, everyone can review (in public repo) and make changes in code and approve those pull 
requests but only people with permission can merge pull request(most cases owner of repo).

Please remember that if in feature branch we create branch, that new created branch will be 
branch of this branch. But we may not want that because that feature branch will not be approved
but our new branch will be approved. 

After merging, pull request will be closed automatically but we may need to delete branch.

We can add contributor to our project by visiting contributors page in repo of github page.

We we add new contributor, contributor get notification and in case of accepting our offer, 
will be granted to act some actions which only owners can do.

By default contributors can merge pull requests by themselves, but it may be need to add some 
min number of approvals before merging (which would be good practice).

These restrictions called rules in Github. In order to add rules(restrictions) we need to visit 
/settings/branch_protection_rules/new and in this page we can add restrictions.

Require pull request reviews before merging - we say pull request is mandatory. We can also 
add number of approvals here.

Dismiss stale pull request approvals when new commits are pushed - when contributor changes its code,
counter will count from 0 again. By this we prevent bad intention. 

Remember owner of repo can merge in any case (remember this is merging as a administrator).
But as a contributor, developer cannot merge before approval (one needs a least one approval). 

Git issues are kinda description of intended, future features. We can also reference in our comment 
or reviews to this issue, by this in issue history we will also see notification about mentioning of
this issue in the files where we referenced. 






