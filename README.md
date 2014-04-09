fsg-github-demo
===============

This is where I'll be uploading/writing/editing the git/github tutorial that I'll be presenting to WVU Free Software Group.


GitHub:

*-https://guides.github.com/

*-https://help.github.com/categories/54/articles

git:

*-http://git-scm.com/doc

*-http://gitref.org/

*-http://try.github.io/levels/1/challenges/1 



**Introduction**

- Who am I?

- What am I gonna talk about?

  - git and GitHub.

- What is git/Github


**git basics**

  - git init projectname

  - cd project name

  - create some files
  
  - git status
  
  - git add filename (or add . to add the whole directory you're in locally)
  
  - git commit -m "Why I'm making a change"  (-m for commit message)
  
**GitHub basics**

  - Create a GitHub account  (www.github.com)
  
  - Create a new repository. Click the + at the top of the page

    - Make it public, Add a readme. Add a license.
    
  - Local vs Web-based
  
    - git clone https://www.github.com/username/reponame - You can clone this repo to your local machine, and work             locally or on the web.
    
    - You can push back to github from both.

  - Creating a repo from your local machine
  
    - git remote add origin https://www.github.com/username/reponame.git
      - makes the url the origin
    - git push -u origin master   (-u for set upstream)
      - pushes your repo/changes to that origin
      - enter username / password
      - maintains your history from your local machine (time stamp, etc. If you created/modified the files yesterday it'd         say in GitHub you created them yesterday.

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
       -SHA-1 is a type of compression. Every change in git is compressed and assigned a SHA-1 hash to make git       
       -lightweight
     - If you click it will bring you to that specific commit.
       -You or any other user can also comment on specific commits. 
     - You can @mention people to bring stuff to their attention.

**No privilege needed for the above, you don't NEED write-access to a repository that isn't yours.**

**Dashboard: Blame/Raw, Wiki, Graphs, Network**

**Issues**

  - To file bugs, ask a question, etc
  
    - Click "Issues"
    - Click "New Issue"
