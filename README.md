Practice files for acloudguru

git initi (create repo)
git status (compare working directory, staging, and current branch)
git add (add changes from working directory to staging)
git commit (commit changes from staging to current branch)
	-m (optional) include a message with the commit (otherwise git opens a text editor)
git config (set or get configuration)
git log (show history of commits)
	-all
		show all logs
	<commit ID>
	<branch name>
	--author "<name>"
		show all logs for author <name>
	--oneline
		displays condensed output

/==================\
	Branches
====================================================
	git branch
		return list of branches with active branch flagged
		-c <name>
			Create a branch with specified <name>
		-v
			show latest changes to all branches
	
	git checkout <branch name>
		switch to desired branch
		-b <name>
			Create and set new branch to HEAD
			
	git stash
		take a snapshot of current changes
		
	git stash list
		list the stashes
		
	git stash pop
		basially git status but for stashes
====================================================