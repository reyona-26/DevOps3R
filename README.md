What is Git?
Git is a DevOps tool that is used as a version-control system for tracking the changes happening in system files and coordinating the work on those files among a group of people. 
In the software development field, Git is used in source code management and for tracking the changes made in any file.
•	Git is a distributed version control and source code management system with an emphasis on speed.
•	It is a repository used to manage projects, the set of files, as they change over time.
•	Using Git, every code change or commit we make gets updated in the development code of a project.
Process Flow
It shows the process flow with components used to perform certain tasks:
•	Plan: It can be created or deleted by itself based on the updates in the source repository.
•	Code: It is the statement written to perform a task in a repository.
•	Shared repository: It is the repository that is shared among several members in order to perform a task.
•	Continuous integration: It helps in updating a repository with the changes made in the code and provides integration with the changes, time to time.
•	Build: It is used to manually build products and dependencies to Git.
•	Configuration management: It is a process of tracking and controlling the changes made in a system.
•	Deploy: Deploy is the process of pushing the code to a remote server.
 
 
Version Control
Version control is the management of changes made to the code, documents, programs, large sites, and other information. The changes are termed as versions.
A version control system (VCS) is used to perform the following:
•	It allows developers to work simultaneously.
•	VCS does not allow overwriting each other’s changes.
•	It maintains a history of every version.
There are two types of version control systems:
•	Centralized VCS
•	Distributed VCS
Our DevOps tool, Git falls under the category of distributed VCS.
Life Cycle
 
Git and GitHub
Git is a VCS that supports distributed nonlinear workflows by providing data assurance for developing quality software.
Its features are as follows:
•	Distributed: A distributed development of code
•	Compatible: Works with existing systems and protocols
•	Non-linear: Allows the non-linear development of code
•	Branching: Easy to create and merge branches
•	Lightweight: Lossless compression
•	Speed: Faster than the remote repository
•	Open-source: A free tool and hence economical
•	Reliable: Not viable to any loss of data upon crashes
•	Secure: Uses SHA1 and checksum
Git Operations and Commands
Git Configuration
•	For the initial configuration of username, email, and code highlighting (optional):
$git config -- global user.name”firstname lastname”
$git config -- global user.email” abc123@abc.com”
$git config -- global color.ui true (enables code highlights)
$git config --list
Initializing Git
•	To initialize:
•	1 st create one directory after installing the git and than initialize the git in the directory:
$git init
•	To know the status:
$git status
Adding and Removing Files
•	To add a file:
$git add<filename>
OR
$git add .
•	To add multiple files:
$git add<filename> <2nd filename> <3rd filename>
•	To add all the updated files:
$git add --all ( use -A instead of -all too )
•	To remove files:
$git rm -r <filename>
OR
$git rm -rf*<filename>
Committing Changes
•	To pass a message, use ‘commit’ with ‘-m’:
$git commit -m “body_of_message”
Or
$git commit -m “This is my firstcommit”

•	To amend the last commit or the last message:
$git commit --amend -m “new_message”

Pushing and Pulling
Here, a remote repository typically represents a remote server or a Git server.
•	To create a remote repository via GitHub, go to:
https://github.com/YourUsername/appname.git
•	To add a link:
$git remote add origin<link>
•	To push files:
$git push -u origin master
Or
$git push origin master

•	To clone files:
$git clone <clone>
Command	Description
git log	To view the changes made
View changes	To view changes (in detail)
git diff [source branch] [target branch}	To preview changes before merging
	Inspection and Comparison
 Following are the branching and merging commands for GIT :
Command	Description
git branch	To list branches
git branch -a	To list all the branches
git branch [branch name]	To create a new branch
git branch -d [branch name]	To delete a branch
git push origin –delete [branchName]	To delete a remote branch
git checkout -b [branch name]	To create a new branch and switch to it
git checkout -b [branch name] origin/[branch name]	To clone a remote branch and switch to it
git checkout [branch name]	To switch to a branch
git checkout –	To switch to the branch last checked out
git checkout — [file-name.txt]	To discard the changes made to a file
git merge [branch name]	To merge a branch into an active branch
git stash	To stash the changes in a dirty working directory
git stash clear	To remove all the stashed entries
Command	Description
git push origin [branch name]	To push a branch to a remote repository
git push -u origin [branch name]	To push the changes made to a remote repository (-u remembers the branch for the next use)
git push origin –delete [branch name]	To delete a remote branch
git pull	To update a local repository to the newest commit
git pull origin [branch name]	To pull the changes from a remote repository
git remote add origin ssh://git@github.com/[username]/[repository-name].git	To add a remote repository
git remote set-url origin ssh://git@github.com/[username]/[repository-name].git	To set a repository’s origin branch to SSH
ADDITIONAL NOTES :
Git Commands
Git is a free, open-source distributed version control system tool designed to handle small to very large projects with speed and efficiency. It has steadily grown from just being a preferred skill to a must-have skill for multiple job roles today. Git has become an essential part of our everyday development process.
In this Git commands tutorial, let’s talk about the top 18 Git commands that are useful for working with Git.
•	git init
•	git add
•	git commit
•	git status
•	git remote
•	git push
•	git clone
•	git branch
•	git checkout
•	git log
•	git stash
•	git revert
•	git diff
•	git merge
•	git rebase
•	git fetch
•	git reset
•	git pull
1. git init
Usage: git init [repository name]
We have to navigate to our project directory and type the command git init to initialize a Git repository for our local project folder. Git will create a hidden .git directory and use it for keeping its files organized in other subdirectories.
 
 
2. git add
Usage (i): git add [file(s) name]
This will add the specified file(s) into the Git repository, the staging area, where they are already being tracked by Git and now ready to be committed.
 
Usage (ii): git add . or git add *
This will take all our files into the Git repository, i.e., into the staging area.
 
We can use this command as git add -A as well.
Note: We will have to commit our files after we add them to the staging area.
 3. git commit
 Usage: git commit -m “message”
This command records or snapshots files permanently in the version history. All the files, which are there in the directory right now, are being saved in the Git file system.
 
 
4. git status
Usage: git status
This command will show the modified status of an existing file and the file addition status of a new file, if any, that has to be committed.
 
5. git remote
Usage: git remote add origin “[URL]”
Once everything is ready on our local system, we can start pushing our code to the remote (central) repository of the project. For that, follow the below steps:
Step 1:
(1) Login to the GitHub account if the account already exists (If not, sign up on github.com)
(2) Click on New
 
Step 2: Now, we have to create a new repository. Provide a name to our repository, select the privacy of the repository as Public, and then click on Create repository
  
Once we are done with filling up the new repository form, we would land on a page as follows:
 
Step 3: Click on the Copy icon on the right side of the URL box of the Github repository to copy the link and paste it as shown below:
git remote add origin “URL”
Now, we are ready to operate the remote commands in our repository that we have just created.
 
6. git push
Usage: git push origin [branch name]
Suppose, we have made some changes in the file and want to push the changes to our remote repository on a particular branch. By using the command ‘git push,’ the local repository’s files can be synced with the remote repository on Github.
 
 
7. git clone
Usage: git clone [URL]
Suppose, we want to work on a file that is on a remote Github repository as another developer. How can we do that? We can work on this file by clicking on Clone or Download and copying the link and pasting it on the terminal with the git clone command. This will import the files of a project from the remote repository to our local system.
(1) The below screenshot shows from where to copy the link:
 To create a local folder, we have to use the following command:
mkdir [directory- name]
cd [directory- name]
git clone [URL]
Now, paste the copied link along with the git clone command as shown below:
 Note: Here, we don’t have to use the git remote add origin command because we have already cloned the remote repository in the local directory. Now, if we push any new file, it knows where it has to go.


8. git branch
Usage (i): git branch [name-of-the-branch]
When multiple developers are collaborating on a project or repository, branches become essential for managing different workspaces. Using this command, we can create a new branch (for example, ‘branch1’). This allows developers to work independently on their respective branches, making changes and commits without affecting the main branch or other branches.
 
Usage (ii): git branch -D [name-of-the-branch]
Likewise, to delete a branch, we utilize the “git branch -D” command. This enables us to remove a specific branch (e.g., ‘name-of-the-branch’) that is no longer needed, cleaning up the repository and reducing clutter.
  
 
9. git checkout
Usage (i): git checkout [name-of-the-new-branch]
This command allows us to switch to an existing branch within our repository. It facilitates navigating to the desired branch, enabling us to add new files, make changes, and commit those files within that specific branch.
 Usage (ii): git checkout -b [name-of-the-new-branch]
This command serves a dual function. Firstly, it creates a new branch with the given name (for example, ‘branch2’). Secondly, it immediately switches our working environment to that newly created branch. This allows us to seamlessly begin working within the newly created branch, making it convenient to add files, make modifications, and commit changes exclusively within that branch.
 
10. git log
Usage (i): git log
The “git log” command is handy when we want to examine the detailed log of every commit in our repository. By executing this command, we can view the log specific to the branch we are currently in. Additionally, we can use “git log -3” to display the last three logs.
 
Usage (ii): git log –graph
For a visual representation of the commit history, we can utilize “git log –graph”. This option presents the commit-graph, showcasing the branching and merging of commits
 
Usage (iii): git log –graph –pretty=oneline
To further customize the output, we can use “git log –graph –pretty=oneline”. This format displays the commit graph along with a concise one-line description for each commit.
 
 
11. git stash
Usage (i): git stash
This command can be used when we want to save our work without staging or committing the code to our Git repository and want to switch between branches.
 
Usage (ii): git stash -u
This command is used when we want to stash the untracked files.
 
Usage (iii): git stash pop
This command is used when we are back on our branch and want to retrieve the code.
 
12. git revert
Usage: git revert [commit id]
The git revert command can be considered as an ‘undo’ command. However, it does not work as the traditional ‘undo’ operation. It figures out how to invert the changes introduced by the commit and appends a new commit with the resulting inverse content.
 
 
13. git diff
Usage: git diff [commit-id-of-version-x] [commit-id-of-version-y]
Diffing is a function that takes two input datasets and outputs the changes between them. The git diff command is a multi-use Git command which, when executed, runs a diff function on Git data sources. These data sources can be commits, branches, files, and more. The git diff command is often used along with the git status and git log commands to analyze the current state of our Git repository. We use git log to get the details of commit IDs.
Let’s compare the working directory with the index as shown below:
 
 
14. git merge
Usage: git merge [another-file-name]
This command will combine multiple sequences of commits into one unified history. In the most frequent use cases, git merge is used to combine two branches. The git merge command takes two commit pointers, usually the branch tips, and finds a common base commit between them. Once it finds a common base commit, it will create a commit sequence.
 
 
15. git rebase
Usage: git rebase [base]
Rebase is the process of moving and combining a sequence of commits to a new base commit. Rebasing is changing the base of our branch from one commit to another, making it appear as if we’ve created our branch from a different commit. Internally, Git accomplishes this by creating new commits and applying them to the specified base. It’s very important to understand that even though the branch looks the same, it is composed of entirely new commits.
The git rebase command performs an automatic git checkout <branch> before doing anything else. Otherwise, it remains on the current branch.
 
Consider a situation where we have branched off from the master and have created a feature branch, but the master branch is still having more commits. We want to get the updated version of the master branch in our feature branch, keeping our branch’s history clean, so that it appears as if we are working on the latest version of the master branch.
Note: We don’t rebase public history. We should never rebase commits once they are pushed to a public repository. Why because the rebase would replace the old commits with the new ones, and it would appear that a part of our project history got abruptly vanished.
 
16. git fetch
Usage: git fetch
When we use the command git fetch, Git gathers any commit from the target branch that does not exist in our current branch and stores it in our local repository. However, it does not merge it with our current branch.
 
In situations where we want to keep our repository up to date but are concerned that updating our files might lead to issues, a specific technique comes to the rescue. To integrate the commits into our master branch, we use the merge feature. This feature actively retrieves all the branches from the repository and then proceeds to download all the required commits and files from another repository. It ensures that our repository remains current while mitigating the risk of potentially breaking our ongoing work.
 
17. git reset
Usage: git reset –hard [SOME-COMMIT]
We use this command to return the entire working tree to the last committed state.
 
This will discard commits in a private branch or throw away the uncommitted changes!
Here, we have executed a ‘hard reset’ using the –hard option. Git displays the output indicating that the HEAD is pointing to the latest commit. Now, when we check the state of the repo with git status, Git will indicate that there are no pending changes (if any prior addition of a new file or modification of an existing file is done before using the ‘git reset –hard’ command). Our modifications to an existing file, if not committed, and the addition of a new file, if not staged, will be destroyed. It is critical to take note that this data loss cannot be undone.
If we do git reset –hard [SOME-COMMIT], then Git will:
•	Make our current branch (typically master) back to point <SOME-COMMIT>
•	Make the files in our working tree and the index (“staging area”) the same as the versions committed at <SOME-COMMIT>
 
18. git pull
Usage: git pull origin master
The git pull command first runs ‘git fetch’ which downloads the content from the specified remote repository and then immediately updates the local repo to match the content.
 

19. Git Ignore :
.gitignore` file is used to specify files and directories that should be ignored and not tracked by version control. Here are some basic commands and steps for using `.gitignore`:

1. **Creating a `.gitignore` file:**
   You can create a `.gitignore` file in the root directory of your Git repository using a text editor. Make sure the filename is exactly `.gitignore`.

2. **Adding patterns to ignore:**
   Inside the `.gitignore` file, you can add patterns that describe the files or directories you want to ignore. Each pattern is placed on a separate line. Patterns can include wildcards.

   Example `.gitignore` content:
   ```
   # Ignore compiled binaries
   *.exe
   *.o

   # Ignore log files
   *.log

   # Ignore a directory
   /build/
   ```

3. **Ignoring a specific file or folder:**
   To ignore a specific file, just add its filename or path to the `.gitignore` file.

   Example `.gitignore` content to ignore a file named "config.ini":
   ```
   config.ini
   ```

4. **Ignoring certain types of files:**
   You can use wildcards to ignore specific types of files. For example, `*.log` will ignore all files with the ".log" extension.

5. **Ignoring files in a directory:**
   To ignore files in a specific directory, you can use a pattern like `/foldername/`. For instance, `/build/` will ignore any files in a directory named "build."

6. **Ignoring files globally:**
   You can set up global gitignore rules that apply to all your repositories. Use the `git config` command:

   ```
   git config --global core.excludesfile ~/.gitignore_global
   ```

   Then, create a `~/.gitignore_global` file with your global ignore patterns.

7. **Applying `.gitignore` changes:**
   After editing the `.gitignore` file, the changes won't affect files already tracked by Git. You'll need to remove the cached entries to apply the changes:

   ```
   git rm -r --cached .
   git add .
   git commit -m "Update .gitignore"
   ```

Remember that `.gitignore` only affects files that are not yet tracked by Git. If a file is already tracked, you need to explicitly remove it from version control using `git rm` if you want to stop tracking it.

Make sure to review and adjust your `.gitignore` file to suit your project's needs and avoid accidentally ignoring important files.
