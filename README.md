#Git basic commands

#Configure the author name and email address to be used with your commits.
	git config --global user.name "Sam Smith"
	git config --global user.email sam@example.com
#Create a new local repository
	git init
#Check out a repository
	git clone username@host:/path/to/repository
#Add files
	git add <filename>
	git add *
#Commit
	git commit -m "Commit message"
#push
	git push origin master
#status
	git status
#Connect to a remote repository
	git remote add origin <server>
#checkout to a new branch
	git checkout -b <branchname>
#checkout to a new branch
	git checkout <branchname>
#delete branch
	git branch -d <branchname>
#Push the branch to your remote repository
	git push origin <branchname>
#Push all branches to your remote repository:	
	git push --all origin
#Delete a branch on your remote repository:	
	git push origin :<branchname>
#Fetch and merge changes on the remote server to your working directory
	git pull
#To merge a different branch into your active branch:	
	git merge <branchname>
#View all the merge conflicts
	git diff
#View the conflicts against the base file:
	git diff --base <filename>
#Preview changes, before merging:
	git diff <sourcebranch> <targetbranch>
#After you have manually resolved any conflicts, you mark the changed file:	
	git add <filename>
#You can use tagging to mark a significant changeset, such as a release:
	git tag 1.0.0 <commitID>
#Push all tags to remote repository:
	git push --tags origin
