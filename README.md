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

- Who am I?

- What am I gonna talk about?

  - git and GitHub.

- What is git/Github


1. git basics

  - git init projectname

  - cd project name

  - create some files
  
  - git status
  
  - git add filename (or add . to add the whole directory you're in locally)
  
  - git commit -m "Why I'm making a change"
  
2. GitHub basics

  - Create a GitHub account  (www.github.com)
  
  - Create a new repository. Click the + at the top of the page

    - Make it public, Add a readme. Add a license.
    
  - Local vs Web-based
  
    - git clone https://www.github.com/username/reponame - You can clone this repo to your local machine, and work             locally or on the web.
    
    - You can push back to github from both.

  - Creating a repo from your local machine
  
    - git remote add origin https://www.github.com/username/reponame.git
      - makes the url the origin
    - git push -u origin master
      - pushes your repo/changes to that origin
      - enter username / password
      - maintains your history from your local machine (time stamp, etc. If you created/modified the files yesterday it'd         say in GitHub you created them yesterday.

3.  Fork / Clone 

  - Cloning/Forking makes an entire copy of a repo.
