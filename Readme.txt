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