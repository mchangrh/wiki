# selfhosted static github pages site

- no additional git server
- no githooks
- no CI/CD
- no fancy UI

## Instructions
1. install git
2. set up git user
    1. useradd... (will change later)
    2. `sudo su - git`
    3. set up ssh keys
3. create your directory structure  
  this will be the directory structure or path of your git address  
  `mkdir cool-project`
4. prepare git  
   personal preference  
   `git config --global init.defaultbranch=main`  
   allow pushing to checked out branch  
   `git config --global receive.denycurrentbranch=updateInstead`
5. prepare remote directory  
   `cd cool-site && git init`
6. add remote and push  
   `git remote add server git@server.example.com:cool-site`  
   `git push -u server main`
7. configure [webserver] to point at /home/git/cool-site
