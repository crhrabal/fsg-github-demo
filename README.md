fsg-github-demo
===============

This is where I'll be uploading/writing/editing the git/github tutorial that I'll be presenting to WVU Free Software Group.

NOTE: This lecture is not supposed to cover all things git/GitHub. This will get you on the right track, but there is a wealth of information in the documentation below. The git/GitHub docs below, along with the man pages within the git program are the best places to go for more info.

**Documentation:** 

  - GitHub:

    - https://guides.github.com/

    - https://help.github.com/categories/54/articles

  - git:

    - http://git-scm.com/doc

    - http://gitref.org/

    - http://try.github.io/levels/1/challenges/1 





**Introduction**

- Who am I?

- What am I gonna talk about?

  - git and GitHub.

- What is git/GitHub?

  - *git* is a distributed version control system. It allows for a person to track changes to documents, and allows for      multiple people to easily collaborate and follow the historical information. It differs from other version control       systems in that it allows most work to be done locally because of the very small footprint that git takes up in terms     of disk space. All historical information about files, including the files themselves, are stored in what is called a     *repository*.
  
  - *GitHub* is a free hosting service for git repositories. A lot of the features from git are combined in an easy to       use web interface that is a good collaboration tool for git repositories. Within open source communities there are       often people scattered all over the world working on huge projects at the same time. That'd be impossible without        things like git/GitHub. People like you and me can get involved in huge open source projects by just submitting a        code review (we'll call this a pull request later)

- Why should I care?

  - Open Source Software is awesome. If you want to get involved with open source, there is probably a good chance you       will be using git at some point in your life. A vast majority of open source projects use git, and a lot of them use     GitHub to host as well.
  
  - GitHub is a good resume - A lot of jobs are looking for practical experience working with a team. You can show           employers these things in a way that says more than you get from a good reference.
   
  - A lot of employers are beginning to switch to git over older tools like svn, mercurial, etc. Nonetheless, if you are     working as a developer in any company, you WILL be using some type of version control, so git in itself is a good        skill to put on your resume.
  
  - Linus Torvalds, the creator of the Linux Kernel, created git!
  
**git basics**

  - Have git installed - It's available (free and open source) for Mac, Windows, and Linux, and the interface is the same     no matter which version you install

    - Typing "git help" in terminal gives a list of commands
    
    - Typing "man git-command" will bring up internal documentation on a particular command. 
    
      - For instance, the man page for "git help" is "man git-help"
    
  - git init projectname

  - cd project name

  - Create some files
  
  - git status
  
  - git add filename (or add . to add the whole directory you're in locally)
  
  - git commit -m "Why I'm making a change"  (-m for commit message)
  
**GitHub basics**

  - Create a GitHub account  (www.github.com)
  
  - Create a new repository. Click the + at the top of the page

    - Make it public, Add a readme. Add a license.
    
  - Local vs Web-based
  
    - git clone https://www.github.com/username/reponame - You can clone this repo to your local machine, and work             locally. 
    
    - Once you create a repo, you can add/edit files, folders on the web as well.
    
    - You can push back to github from both.

  - Creating a repo from your local machine
  
    - git remote add origin https://www.github.com/username/reponame.git
      - makes the url the origin
        -Origin can be local, github, or a private server for which you have write-access. You can also change the origin          at any time. Origin doesn't mean "where it started," though it is often used that way. Origin just sets what you          want your remote repository to be. You can have multiple remote repositories.

    - git push -u origin master   (-u for set upstream)
      - pushes your repo/changes to that origin
      - enter username / password
      - maintains your history from your local machine (time stamp, etc. If you created/modified the files yesterday it'd         say in GitHub you created them yesterday.

  - Deleting / Renaming a repo 
  
    - Click the screwdriver and wrench on the right side of the screen.
     
      - There is a space to rename the repository in the settings menu.
    
      - You can click "delete this repository" at the very bottom of the next screen. It warns you, once you delete it,          that it's gone forever (Back it up locally if that's important!)

**Fork / Clone**

  - Cloning/Forking makes an entire copy of a repo.
  
    - Click Fork button - Area at top shows you that your fork is your personal copy of the repo. You can make any
      changes and it does not affect the original.
    
    - Click on "classroom" folder
      - Click + button to add a file username.md
        - Add your name
        - Commit file
  
    - A file is created in your fork. 
    
  - Click Pull Request
    - Will show you preview of your changes
    - Add a message, Click Send Pull Request
  
  - The owner of the repo can click Pull requests on the right of the screen
    - If you click on a pull request, you or all other uses can add comments to specific pull requests.
      - Comments update in real-time. 
      - A pull request is a code review, asking someone to merge your changes into their repo.
  
**Commenting**

  - Click commits on a pull request or at the top of a repo
     - Click SHA-1 number
       - SHA-1 is a type of compression. Every change in git is compressed and assigned a SHA-1 hash to make git       
         lightweight
     - If you click the SHA-1, it will bring you to that specific commit.
       - You or any other user can comment on specific commits. 
     - You can @mention people to bring stuff to their attention in a comment.

**No privilege needed for the above, you don't NEED write-access to a repository that isn't yours.**

**Dashboard: Blame/Raw, Wiki, Graphs, Network**

**Issues**

  - To file bugs, ask a question, etc
  
    - Click "Issues"
    - Click "New Issue"

**Back to git** - TODO

  - Cloning
  
    - Local
    
    - Remote
  
  - Fetching
  
    - Local 
    
    - Remote
  
  - Merging

    - Local
    
    - Remote 

  - Pushing
 
   - Local
   
   - Remote

**Branching and Merging (And the conflicts that arise)** 
(This could really be it's own lecture, especially if I talk about plumbing, like what's in the .git folder)

  - If I make changes to this file and then you decide you want to have the latest changes.
  
    - In git 
    
      - git fetch origin
      - git merge master
      
    - On GitHub
    
      - Go to that repo and click pull request
      - Merge changes
  
