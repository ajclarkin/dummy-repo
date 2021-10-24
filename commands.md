### List of Useful Git Commands ###

#### Cloning a repository ####
`git clone <url>` where the url comes from the main page of the repository


#### Adding and updating files ####
- `git add <filename>` specify the file to add at the next commit (aka stage the file)
- `git add .` adds all the files in the directory
- `git status` lists the files staged for the next commit
- `git commit -m <comment>` commits the staged files


#### Branch and merge ####
- `git branch` lists the branches. * denotes the current branch
- `git branch <branch-name>` creates a new branch
  - `-a` lists all branches, `-r` lists remote branches
- `git checkout <branch-name>` switches to another branch

Note that the local repo might not be up to date with the online version. `git fetch` will update that and so you might need to do this before `branch` or `checkout`.


#### Updating with online repo ####
- `git pull` updates the local branch to match what's online
- `git push` pushes the local commits back up to the online repo
- `git push -u origin <branch-name>` pushes a new local branch up to the online repo
