# gittutorial

## Basic commands for Git Version Control System for beginners

First of all lets configure our git for our tutorial. We will just simply add our Name, Email and configure in such a way that git only asks us the credentials for the first time and stores it for future use. So, you will only do this if you are in your own personal devices.

### **1) Configure git**:
> git config --global user.name "&lt;Your Name&gt;"  
> git config --global user.email "&lt;Your Email&gt;"  
> git config --global credential.helper store

Final command basically stores your credentials after you first enter your credentials to make some remote changes.

**You can work on your projects linking locally and remotely and making changes by two ways:**

### **1) Clone a repository**:
> git clone &lt;full-link-of-github-repository&gt;

### **2) Create a new repository locally and pull it from remote repository**:
Creating a new repository is simple. First you need to create a repository in github and then create a new directory with the same name locally. Then inside that folder you need to run these commands:
> git init  
> git remote add origin &lt;full-link-of-github-repository&gt;  
> git pull origin master

First you initialize the git inside your directory or say local repository then you add origin of the remote repository which is the github link to your repository. Finally you pull your repository from remote server which is the github server.

Here 'origin' is the alias for the server URL. It is the default alias set by git. You can also change it using command as:
> git remote rename origin &lt;newalias&gt;

And you can use following command with new alias to pull the remote repository:
> git pull &lt;newalias&gt; master

**After you have used one of the above methods to have a copy of remote repository you can work on it locally and make edits and commit it to remote repository. Some of the useful commands along with those commands are:**

Suppose you made some changes in a file or some files you just fetched from remote repository (just refering to the thing we did in last step). Then you would want to have the same changes in your remote repository. To do that you push your changes to the remote repository.
But first you need to specify which file or files you want to push by:
> git add &lt;file-name&gt;  

If you want to add all the files that is in the local repository (refering to your project directory) you do it by:
> git add .  

"." just says you want to add all of the files in the current directory.

Then you need to commit these changes locally. You also need to add a commit message. Both things can be done with the same command by:
> git commit -m "&lt;Your commit message&gt;"  

-m flag is used for adding commit message.

Finally you need to push your changes to the remote repository by:
> git push origin master

You need to provide your credentials if this is your first time using git following this tutorial. Once you provide credentials here it will be saved and used for future purpose if you followed from the beginning of this tutorial.
