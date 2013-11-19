NC State Github training
=========
Notes:
Reveal js - open source presentation framework

**git --version**

**git init .**   

**git config user.name**   
view current username in global config  

git config --global user.name "Rohit Kandhal"  
git config --global user.email "rohit_kandhal@yahoo.co.in"  
git config -global color.ui.auto  

**git add .**    
	1. Move file to staging area, do it after every change  
	2. To go back from stage - use reset.  
	3. '.' -> Add recursively new and modified files  

git commit -m "Initial Commit"  
	1. Each commit has a commit ID generated using SHA-1 algorithm

git log  
git log --format=raw (Indicates parent (or parents) commit)  
git log --graph  
git log --graph --decorate  
git log --graph --decorate --oneline  
git log --graph --decorate --oneline --all  

git config --global alias.lol "log --graph --decorate --oneline"  
	1. Create alias of a command

git branch  
	1. view all branches and current selected branch)  
git branch -a  
git branch -r  

git branch feature  

git checkout feature (switch to difference branch)  

_Before merging, go to the target branch using checkout. Merge is equivalent to commit._   

git checkout master  
git merge feature(branch name) -m "Merged"  

_After merging there is no point in keeping the "branch"_    
git branch -d feature  
	1. Note: deleting a branch does not deletes commit history  

git remote add origin https://github.com/rohitkandhal/git-train.git  
 
git remote  
> Address look up

git remote -v

git push --set-upstream origin master  
	1. Push master branch at origin  
	2. 'set-upstream' Connect my local branch's master to origin branch's master  
	
_Every branch has its own master_  
git config push.default  
git config --global push.default  
	1. Different git push strategy  
	
git fetch  
	1. What new commits you have and update the remote branches.  
git pull  
	1. Fetch and then 'Fast-Forward' merge  
	
git config --global credential.helper  

git clone https://github.com/rohitkandhal/nc-state.git  
	1. Create a copy or clone of fork to work locally  
	
After merge you need to do git add again     
<<<< - ours  
">>>> -  theirs  

git help config  

git remote add teacher https://github.com/githubteacher/nc-state.git  

git reflog
