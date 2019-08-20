<h1 align = 'center'>Working with git</h1>
<hr>

<h3 align = 'center'>Creating a GIT Repository</h3>


1. Create a Repository on GitHub.com

![Github](images/github-create-repo-screen.PNG)


2. Copy the link shown below
![Github](images/git-create-repo-empty-screen.PNG)
3. Navigate to the folder in which you whish to create the repository
1. Enter the command `git init` This initializes the local repository on YOUR COMPUTER .
2. Enter the command `git add remote origin <github-url>` (This is hte command we copied from the website) This will set the upstream of your local repository connecting it to the online repository.
3. Enter the command `git add -A` This tracks all the files inside of the added and deleted files inside of the local repository.
4. Enter the command `git commit -m '<message>'` This commits the current changes to your local repository.
5. Enter the command `git push origin master` This pushes your local repository to your online repository.

![Terminal](images/git-finished-painted.png)

<hr>
<h3 align = 'center'>Updating an existing repository</h3>

1. `git add -A` This tracks all the files inside of the added and deleted files inside of the local repository.
2. `git commit -m '<message>'` This commits the current changes to your local repository.
3. `git push origin master` This pushes your local repository to your online repository.

<hr>

<h3 align = 'center'> Common Errors</h3>

![GitBash](images/no-tracking-info.PNG)

* <h4>No tracking info</h4> 
    1. Fix: Use `git pull origin master` instead.

![GitBash](images/git-repo-in-repo.PNG)

* <h4>You created a git repository inside of your current repository</h4>

    1. Navigate to the child git directory (to find it check folders and see if you can use the command `cd .git`)

    2. Use the command `rm -r .git -f` to un-initialize the inner repository

    3. Add, Commit, Push as usual

![GitBash](images/updates-rejected.PNG)

* <h4>Updates were rejected</h4>

    1. `git pull origin master`
    2. Fix any merges if they appear
    3. `git push origin master`

* <h4>I can't pull the class repository</h4>

    1. `git reset --hard`
    2. `git pull origin master`