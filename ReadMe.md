#### GIT Commands:


##### Initial Setup

```
git init
git remote add origin https://github.com/suresh12391/spring-rabbitmq.git
git config user.name "Suresh Arumugam"
git config user.email abc@gmail.com

git config --global user.name "Suresh Arumugam"
git config --global user.email abc@gmail.com

git config --list --show-origin

git remote set-url origin https://github.com/suresh12391/spring-rabbitmq.git
git remote -v
```



| Command | Description |
| ------- | ----------- |
| `git clone https://gitlab.com/abcd/123.git` | To clone a repo from remote |
| `git branch` | To list the branches |
| `git status` | To check the current branch and list status |
| `git checkout master` | To move into master branch |
| `git checkout -b 123-new-branch` | Create new branch from master |
| `git checkout 123-new-branch` | Move to 123-new-branch for the implementation |
| `git add file.txt` | Stagign the file changes |
| `git commit -m "Added new file"` | Commiting the changes |
| `git push origin 123-new-branch` | Pushing the changes to remote server |
| `git gui` | Graphical User Interface Tool for the Git CLient |
| `git branch -D 123-new-branch` | Delete the 123-new-branch branch | 
| `git fetch origin 345-diff-branch` | Pulling the 345-diff-branch branch from server |
| `git log` | To see history of commits in reverse order |
| `git fetch origin xyz-new-branch` | To fetch the remote branch first time |
| `git pull origin xyz-new-branch` | To pull latest code from remote |
| `git merge master` | To merge the master code into the current branch |
| `git merge --abort` | Incase to avoid non-commited merge changes. ie, the conflicted merge |
| `git stash list` | List out the already stashed changes |
| `git stash` | To Stash the current changes |
| `git stash pop 0` | To pickup the last stashed changes from the stack |
| `git stash drop 0` | To drop the last stashed changes from the stack |
| `git gc` | To perform GC in GIT |


Git Tag:

```
$ git tag <tag-name> master       # Create a tag from a branch
$ git tag                         # see tag lists
$ git push origin <tag-name>      # push a single tag
$ git push --tags                 # push all local tags 
$  git push --follow-tags         # It pushes both commits and only tags that are both
$ git push --delete origin <tag-name>    # Delete the tag in remote
$ git tag -d <tag-name>          # Delete the tag in local
```

Reference(s):
- https://www.tutorialspoint.com/git/index.htm
- https://www.atlassian.com/git
- https://www.atlassian.com/git/tutorials/setting-up-a-repository
- https://www.freecodecamp.org/news/learn-the-basics-of-git-in-under-10-minutes-da548267cc91/
- http://www.amarinfotech.com/gitlab-vs-github-vs-bitbucket.html
- http://genomewiki.ucsc.edu/index.php/Resolving_merge_conflicts_in_Git

Revert Git Change(s):
- https://opensource.com/article/18/6/git-reset-revert-rebase-commands
- https://stackoverflow.com/questions/927358/how-do-i-undo-the-most-recent-local-commits-in-git
- https://stackoverflow.com/questions/4114095/how-do-i-revert-a-git-repository-to-a-previous-commit


Other Git Commands:
| Command | Description |
| ------- | ----------- |
| `git fetch -p` |  |
| `git branch -vv \| grep ': gone]' \| awk '{print $1}'` | |
| `git branch -vv \| grep ': gone]' \| awk '{print $1}' \| xargs git branch -d` |  |
| `git remote prune origin` |  |
| `git remote prune origin --dry-run` | 
| `git branch --merged >/tmp/merged-branches && vi /tmp/merged-branches && xargs git branch -d </tmp/merged-branches` | |



