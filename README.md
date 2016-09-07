# figures_160929

This repository was created as an exercise in using git and github for PhonLab users. The task is to add a figure that you would like to discuss at the next Lab meeting.

# TL;DR

Create a github account and fork this repository to your account. Clone that repository into the BPM, add your figure, and push the changes to github. Submit a pull request to Susan to add your changes to her repository.

# Again, in more detail

## Create a github account

Go to https://github.com and create an account. We'll assume you can handle this on your own. You can use your @berkeley.edu address or a personal email account when you sign up.

## Fork Susan's main repository

The idea in this step is to create a copy of Susan's repository under your own account on github. This will be a public repository, just like the original.

1. Visit https://github.com/susanlinucb/figures\_160929 in your web browser.
1. Click on the 'Fork' button in the upper right corner.
1. Your fork will be created, and your web browser will automatically redirect to your forked repository. Take note of the url for the next step.

## Clone your repository to your local system

In this step you will make a copy of your fork on your local system. This repository is private unless you take steps to open it to the world.

1. Start the BPM and open a terminal window. Your home directory should be your current working directory.
1. Make a clone under the `src` directory with these commands:
  cd src
  git clone https://github.com/<myusername>/figures\_160929  # url of your fork
1. Now make the repository your working directory:
  cd figures\_160929

Is there a difference between forking and cloning? Not really, both are complete copies of a repository. The word 'fork' is used on github for server-to-server clones and isn't a term used by git itself.

## Add your figure to the repository

The next task is to copy your figure to the repository and commit the changes.

1. Using the command line or file browser, copy your figure to `~/src/figures\_160929`.
1. At the command line, take a look at the changes you have made to the repo:
  git status
1. You should see the name of the file you just added in the 'Untracked files' section of the status message.
1. Tell git to start tracking the file by adding it to the repository, then check the status again:
  git add yourfile.png
  git status
1. Your file should now be in the 'Changes to be committed' section. Commit the change to the repository, including a short message describing the change:
  git commit -m "Added ...'s figure file."
1. Check the status again, which should tell you that you are ahead of 'origin/master' by 1 commit:
  git status

At this point your changes have been committed to your local, private repository only and no one else can see them. Note that in git terminology each repository copy is a repository in its own right, and the use of 'commit' is subtly different than in other version control systems that are not as distributed in character. When you 'commit' in git you make your changes in a repository permanent, and this repository is often (but not always) your local one. These changes do not automatically propagate to other related repositories. In other version control systems (like svn), a 'commit' makes your changes permanent and copies them to the master repository.

## Push your committed changes to your public repository

In order to make your committed changes public you must push them to your public repository on github:

1. Give the command and check the status:
  git push
  git status
1. 
## Add
