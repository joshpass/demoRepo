git config --global user.name "josh.pass"
git config --global user.email "joshpasricha@gmail.com"
git config --global core.editor vim
git config --list

git clone repositorylink
git push --set-upstream origin master #When the current branch master has no upstream branch. (After cloning new repo)
 
git add filename/regex
git add . (Adds all files)

git commit -a (For all added/modified files). Will go into vi to ask for message. #i to insert. Esc to exit. :wq to save
git commit -m "message"
git push
git pull

Stash - Cleans your working directory back to remote branch state, and will store currently going on work into a separate stack. This is for switching work in the middle without committing, but still saving. 
git stash #saves to stack
git stash list #shows all stashes
git stash pop #returns working repo back to the topmost stash state

Misc
git log
git diff
git checkout filename (If screwed up in local repo, Will revert back file to original state, will get back deleted file also)
git commit --amend -m 'new message'
git show commitnumber

Tags
git tag -a 'tagname' -m 'tagdescription' HEAD #HEAD always points to the latest successful commit. Can replace HEAD here with a commit number also
git push tag tagname
git tag -l #View all tags
git show tagname #View details of specific tag
git tag -d tagname #Delete a tag

Branching
git branch new_branch
git branch #View all branches. Shows a asterisk mark before currently checked out branch.
git checkout new_branch #switch branches
git checkout -b test_branch #shortcut to create and switch in one command
git branch -D test_branch #delete branch after switching to master or whatever other branch
git branch -m oldname newname #rename branches
git merge origin/otherbranch