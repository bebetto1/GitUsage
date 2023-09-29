1. To create repository go to github.
2. Create repository
3. Go to the Project folder and run:
   git clone git@github.com:bebetto1/GitUsage.git
4. Add file: readme.md and stage it
   git stage -A
5. Commit files:
   git commit -m "Added readme file"
6. Push files to the repository:
   git push

-----------------------------Change global name and email------------------

1. See current name and email:
   git config --global user.email
   git config --global user.email

git config --global user.name "NewName"
git config --global user.email "NewEmaiil"

-----------------------------How to create your change and push it to the main branch------------------------

1. Create branch for task.
   git checkout -b feature-T43255
2. Commit changes to branch but not push your branch to the remote server.
3. Rebase your branch to the local master (dev or the main branch for development)
   git rebase master
4. Switch to the master branch
   git checkout master
5. Pull the last changes from the server
   git pull
6. Merge changes from local branch.
   git merge --ff-only feature-T43255
7. Push changes to the remote server.
   git push
