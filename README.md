# 🤗 A Friendly Intro to Working with Your Bitbucket via SSH on Windows

  In this tutorial I will show you a quick way to setup your environment to be SSH-ready.

## What is SSH?

  [Wikpedia](https://en.wikipedia.org/wiki/Secure_Shell) says:
  
  *Secure Shell (SSH) is a cryptographic network protocol for operating network services securely over an unsecured network*
  
  * It's a fancy way of saying that you can safely send your data from one place to another. 
  
  * In our case you'll send the data (your code) from your machine to your repository or vice versa :)
  
## Why to even bother?

  * SSH lets you synchronize your local code with your repository in a convenient and quick way. 
  
  * You won't need to drag and drop files, click confirmations and do other tedious stuff anymore. 

## Install Git Bash

  Git Bash is a **command line tool**. Basically, a window, where you can put your commands.
  
  * To instal `git` click [here](https://git-scm.com/downloads)
  
  * Tell the installator that you **want to add git to the context menu** - it will give you very convenient options later!
  
## Generate your ssh key

  You can think about SSH key as your identifier - it let's Bitbucket (or GitHub or any other software that uses SSH) identify you.
  
  To generate your first ever SSH key you need to follow two simple steps:
  
  * ### Open your new friend - Git Bash
    * In any folder (might be just your desktop) click your right mouse button
    * Select `Git Bash Here`
    
  * ### Go to this [link](https://confluence.atlassian.com/bitbucket/set-up-an-ssh-key-728138079.html)
  
    * Find **Set up SSH for Git on Windows**
    
    * Follow the steps there (you can ommit **Step 2** if you feel so - it will work)
    
    🎉 **Congrats!** You just generated your first SSH key! 
    
## Clone your repository

  * Go to your Bitbucket (or GitHub or so...) repository and click `Clone`
  
  * Choose `SSH` option in clone window
  
  * Copy the content of sub-window 
  
  * Paste it into Git Bash 
    
    **HARD PART ALERT :)**: in Git Bash use you don't use `Ctrl + C` and `Ctrl + V` instead use:
    
      * `Insert` to paste (and copy) (I know, I know, but it works 🤔)
    
    **NOTE**: check if what you just copied starts with words `git clone`. If yes just press `Enter`. If no add `git clone` in front of what you just copied and press `Enter`.
    
    You should see something similar to the output below on your screen:
    
    ```bash
    $ Cloning into 'PyTorchExercises'...
    remote: Compressing objects: 100% (3/3), done.
    bash: Cloning: command not found
    remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
    Receiving objects: 100% (4/4), done.

    ```
    
    🎉 **Well done!** You rock!
    
## Using git 

  There are three super-basic git commands:
  
  * `git status` - you check the status of your local repo
  
  * `git add .` - you prepare all your changes (here `.` means *all*) to being commited
  
  * `git commit -m "<some nice descriptive message here>"` - you commit your changes and describe what your changes are 
  
  * `git push` - you send your files to the repository (here is where all that **SSH** hustle pays off! 😊)
  
  * `git pull` - you download the latest version of the code from the repository
  
  To get more familiar with these commands you may want to watch this nice video: https://youtu.be/eL_0Ok_Gkas?t=175
  
  
🎉 **Congrats!!!**

You just learned how to work with bitbucket with SSH. How cool is that? 😃


  
If you want to learn more about version control in general you may like this: https://www.youtube.com/watch?v=0fKg7e37bQE&t=698s
  
  
