# Git Notes

## Local commands
- 'get init' :initialize current folder as a git repository
- 'git clone <URL>' :brings the current git repo from url to current folder
- 'git status' : tells us what we need to know about the repo and its state
- 'git add <FILE>' : adds a file to the staging area
- 'git commit' : opens a text editor to write a commit message
	- 'git commit -m': writes MESSAGE as a commit without a text editor
- 'git log': shows the log of our commits
	- 'git log --oneline': shows shorter oneline commit
- 'git diff': compares current uncommited state to last known commited state

- 'git diff --staged': runs git diff between theg area and last known state
- 'git diff HEAD ~': compares HEAD with commit number ago (relative)
- 'git diff HASH': compares HEAD with HASH

- 'git restore --source (HASH or HEAD) (FILE)': restore file to HASH or HEAD
	- 'git checkout (HASH OR HEAD) (FILE)': restore file to HASH or HEAD
		- 'git checkout (HASH OR HEAD)': if you forget the file name, you end up in a detached HEAD state
		- 'git checkout main': go back to main
		- 'git switch main': go back to main

## Remote commands
- 'git remote add NAME URL': adds the URL to a remote with NAME
	- NAME by convention is 'origin'
- 'git remote rm NAME': removes the remote called name
- 'git remote -v': look at all the remotes you have
- 'git push WHERE WHAT': pushes the WHAT to the WHERE branch
	- 'git push origin main'
- 'git pull WHERE WHAT': pulls the WHAT branch to WHERE in local computer

## Branches
- 'git branch NAME': creates branch NAME where you are (HEAD)
- 'git switch NAME': moves to the branch NAME
	- 'git checkout NAME': same as above
- 'git switch -c NAME': creates and moves to branch NAME
	- 'git checkout -b NAME': same as above

