# Tech Notes

## Git Commands

### To create a new repository on the command line

echo "# tech-notes" >> README.md  
git init  
git add README.md  
git commit -m "Initial commit"  
git remote add origin https://github.com/ohrsantos/tech-notes.git  
git push -u origin master  


### To push an existing repository from the command line

git remote add origin https://github.com/ohrsantos/tech-notes.git  
git push -u origin master


### To see what is about to be *committed* using git diff with the *--cached* option

git diff --cached


### To see what is about to be *added* using git diff without the *--cached* option

git diff 


### To get a brief summary of the situation

git status

#### more compact way

git status -s

### To unstage

git checkout -- <file(s) or .>

### Revert and delete do previous commit point

git reset --hard <commit id>

### To create a new branch

git checkout -b <branch name>
  
### To merge to master branch

git checkout master or git master
git merge <branch from>

### To delete a branch

git branch -D <branch name>
  
### To keep the file in your working tree but remove it from your staging area  

git rm --cached 

### To remove it from your tracked files (more accurately, remove it from your staging area) and then commit

git rm

### To remove a *changed* file from your tracked files

git rm -f
