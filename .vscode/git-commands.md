GIT COMMANDS

git status

git remote
git remote remove
git remote add origin git@github.com:lindokuhle-mncwabe/FixClient.git
git push -u origin master

git fetch

git branch <new-branch-name>
git checkout -b <new-branch-name> # brings all uncommitted changes to the new branch

git add .
git commit -m "<commit-message>"

git restore .                                         # undo unstaged local changes
git restore hello.c                               # undo unstaged change to specific file
git restore --staged hello.c                # undo staged local changes to specific file

git log main..HEAD
git log --stat main..HEAD

git show <commit-hash>
git show --stat <commit-hash>

git push
git push --set-upstream origin <new-branch-name>
git push --set-upstream azure <new-branch-name>

git diff --cached                     # to see changes that will be applied on the next commit
git difftool                              # to view diff side by side | :qa + Enter to quit difftool
git diftool -- [<file-path>]     # git difftool -- .\infra\gateway-api\main.bicep

# resetting feature branch to main
git checkout main 
git fetch origin                                                                 # maket sure you have the latest state of main branch
git checkout <feature-branch-name>
git reset --hard origin/main
git push origin <feature-branch-name> --force             # be cautious when using git reset --hard and git push --force 
                                                                                         # as they can lead to data loss by discarding commits. 

 
