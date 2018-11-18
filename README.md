# linkit-kaggle-Team #

## Set up working directory ##
1. Open your Terminal 

2. Create a new working directory with `mkdir <dir_name>`

3. Navigate to the directory using `cd <dir_name>`

4. Clone the Github-Repo using `git clone https://github.com/linkit-kaggle/kaggle.git`

## Working with Github ##
- to see which you are working on use `git branch`. The asteriks (*) indicates the current branch.

- to work on your ideas, always create a new branch using 
`git checkout -b <new_branch_name>`

- use `git status` to see what files you changed on your branch, compared to your last commit.

- use `git add .` to stage changes locally 

- then, use `git commit -m "<your-initials>-<commit message>"` to save the changes locally.

- If you want somebody else to be able to work on that particular branch, you have to push it to the remote github repo.
Use `git push origin <branch-name>` to push your last commit to the remote.
The other user can fetch new branches using `git fetch` and then switch to your branch using `git checkout <branch-name>`.
In case you are working on a branch together, use `git pull` on that branch to fetch changes to the files and merge them into your local copy.
Btw, once you first used the `git push origin <branch-name>` command, Git remembers the local-remote relationship. 
Means, next time you want to push changes on that branch, just run `git push`.

- Assume you've been working on a branch called `jb-kaggle-idea` and now want to merge these changes into the master.
Stage and commit the changes on that branch and then switch to you local master by running `git checkout master`.
Now pull new changes from the remote origin master so you stay up to date (`git pull`).
Merge your local branch `jb-kaggle-idea` into you master using `git merge jb-kaggle-idea`.
Git merge always merges the argument branch (in this case `jb-kaggle-idea`) into the branch you are currently on.
If there were no merge conflicts, stage, commit and then push your master to the remote: `git push`. Note that to push from master, you will never have to set up a remote branch manually, as the local-remote relationship was established on the `git clone` command in the beginning. 

- Other users can run `git pull` from their master to import the changes you made.

- Always be careful pushing to the remote master. 

- Naming convention for creating branches and commit messages: 
    1. all lower caps letters
    2. start with you initials 
    3. only for branch-names: separate words with a dash (-) 
    4. follow up with the use of that branch / commit
    5. write commit messages in present
    5. Example: `git checkout -b jb-show-how-branches-are-made`
    6. Example II: `git commit -m "jb - set up readme file"`
 








 









