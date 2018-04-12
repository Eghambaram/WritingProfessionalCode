#Adding an existing project to GitHub using the command line

Simple steps to add existing project to Github.

## 1. Create a new repository on GitHub.
In Terminal, change the current working directory to your local project.

##2. Initialize the local directory as a Git repository.

	git init
	
Add the files in your new local repository. This stages them for the first commit.

	git add .

or:
	
	git add --all

Commit the files that you've staged in your local repository.

	git commit -m 'First commit'


Copy remote repository URL field from your GitHub repository, in the right sidebar, copy the remote repository URL.

In Terminal, add the URL for the remote repository where your local repostory will be pushed.

	git remote add origin <remote repository URL>
	
Sets the new remote:
	
	git remote -v

Push the changes in your local repository to GitHub.

	git push origin master

Pushes the changes in your local repository up to the remote repository you specified as the origin

Add new folder into git repo
	
	git add -f [foldername]



## 2. Working with Git and a Remote Repository.
In Terminal, change the current working directory to your local project.

Apart from our brief tour of GitHub in the preceding lesson, nearly everything we have done with Git and source control was local to our machine. So far in this course, we practiced the following Git commands.

	* git status - checks the state of a repo
	
	* git add - stages updates
	
	* git commit - commits updates
	
	* git checkout - switches branch
	
	* git branch - lists existing branches
	
	* git log - shows commit history
	
	* git pull - This command incorporates the changes from a remote repository into the current branch
	
	* git fetch - the fetch command essentially updates your remote-tracking branch, in this case origin. Performing a git remote -v at your command prompt
	
	* git push - on both the server and your local copy, all managed with the git fetch, git push and git pull commands


##  At the command prompt or terminal window of your machine type the following command

	git clone [URL]


Replace [URL] by pasting from the clipboard. Alternatively, replace [URL] in the command above with a URL in the format https://github.com/<your_github_username_here>/hello-remote.git.
