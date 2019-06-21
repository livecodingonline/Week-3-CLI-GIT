# Using Git

## 1.1 Creating the repository

Using your GitHub account, create a repository to which you can add files. Name the repository as MyFirst. Create a public repository and check the box to create a README file.
You can clone the repository you created with `git clone <URL>` command. This copies the repository from a remote machine and initializes it on your machine.
After you create the repository, the URL of your web page would be something like https://github.com/USERNAME/MyFirst. Replace USERNAME with your username.
You can also try to clone any public repositories on github.com

## 1.2 add and commit
```
#You can propose changes (add it to the Index) using
$git add <filename>
#This is the first step in the basic git workflow.

#To see changed and added files
$git status

#To actually commit these changes use
$git commit -m "Commit message"
```

## 1.3 Pushing changes
```
$git push
```

## 2.1 Initializing repository locally 

The other way is initializing git repository locally. 
```
Create a new directory in your home directory or any other suitable location using
$mkdir hello-world
Enter it
$cd hello-world
and create a new git repository using 
$git init
```

## 2.2 Configure your email and username of Github in the git
```
$git config --global user.email "username@email.com"
$git config --global user.name "username"
```

## 2.3 add and commit (Same as 1.2)
```
#You can propose changes (add it to the Index) using
$git add <filename>
#This is the first step in the basic git workflow.

#To see changed and added files
$git status

#To actually commit these changes use
$git commit -m "Commit message"
```

##2.4 Pushing changes 
```
#If you have not cloned an existing repository and want to connect your repository to a remote server, you need to add it with

$git remote add origin https://github.com/USERNAME/REPOSITORY.git 
Replace the URL with the repository you made before

Now you are able to push your changes to the selected remote server i.e. your remote repository on GitHub.
Your changes are now in the HEAD of your local working copy. To send those changes to your remote repository, execute 
$git push -u origin master
```
# Troubleshooting
You could encounter errors if you do not follow the exact procedure as described above.
```
error: failed to push some refs to 'git@github.com:myrepo.git'

Solution:

$ git pull origin master
```

```
fatal: refusing to merge unrelated histories

Solution:

$ git pull --allow-unrelated-histories origin master
```
