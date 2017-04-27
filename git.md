### connect to remote repo
`$ git clone https://github.com/[remote repo]`

### Check remote origin/upstream:
`$ git remote -v`

### Check all branch
`$ git branch`

### Git add
* `$ git add -A` : stages All.
* `$ git add .`  : stages new and modified, without deleted.
* `$ git add -u` : stages modified and deleted, without new.

### To create a new branch locally and push to remote repo
1. `$ git checkout -b [name_of_your_new_branch]`
### Create the branch on your local machine and switch in this branch
2. `$ git push origin [name_of_your_new_branch]`

### To add some file to your remote repo
1. git clone your repo
2. modify file as you want
2. `$ git add .`
3. `$ git commit -m "some comments"`
4. `$ git push origin [name_of_branch_to_push]`

### Sync your fork
1. git clone your forked repo
2. `$ git remote -v` : check if upstream is set. Upstream is the repo you fork from
3. `$ git remote add upstream [upstream repo]` : if upstream not set
4. `$ git fetch upstream` : download the lastest update as a new branch to your local
5. `$ git merge [newly download branch]`
6. `$ git push origin [branch name]` : update your remote forked repo

