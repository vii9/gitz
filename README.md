#GiT and GiTHuB

### Git Branch
``` 
git branch name_branch
git checkout name_branch
=> git checkout -b name_branch
```
### Pull Resources
```
\*** pull resources from github
$ git pull origin main 
\*** fetch 1 pull request from github into local branch
$ git fetch origin pull/484/head:new_name_branch_local
```
### Merge Commit Using Rebase : n -> 1
```
$ git rebase -i HEAD~2(3)
	:: delete pick(commit) and change 
	- f: No edit commit after rebase
	- s: edit commit after rebase
```
### Delete 1 commit:
```
$ git reset --soft|hard HEAD~1 
    - hard is delete commit and file change
```
### Git stash:
```
	$ git stash push -m"save for me"
	$ git stash list
	$ git stash apply stash@{0}
```
### Git fetch remote branch:
```
	$ git fetch origin worker4:fix-worker4	::NOTE (remote_branch:new_local_branch)
	$ git checkout fix-worker4
```

### Template github pull request
```
### 1. Related Tickets
 * [Redmine#DEEP_APP-24](https://laravel.com)
 
### 2. What's this PR do?
* [x]  add file from worker3
* [x]  create conflict Flag
```
