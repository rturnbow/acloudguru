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
git diff <target_name>..<target_name2>
	show difference between local directory and <target_name> defaults to HEAD; can compare branches, refs, commits, etc
	--cached 
		show difference between staging and target (HEAD default)
		
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

/==================\
	Remote
====================================================
	git remote
		add <remote> <url>
			add a new <remote> at <url>
		-v
			list remote repositories
			
	git push -u <remote> <branch>
		push <branch> to <remote>, and set default upstream for branch
		
	git log --oneline remotes/origin/main
		view log of remote repo
	
	git fetch
		pull down changes from remote repo
	
	git merge
		merge fetched and current repo (may generate conflicts)
		
	git pull
		fetch and then merge
		
	git push
		push code to remote
====================================================
