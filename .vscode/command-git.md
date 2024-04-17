# GIT COMMANDS

git status <br/>

git remote <br/>
git remote remove <br/>
git remote add origin git@github.com:lindokuhle-mncwabe/FixClient.git <br/>
git push -u origin master <br/>

git fetch <br/>

git branch <new-branch-name> <br/>
git checkout -b <new-branch-name> # brings all uncommitted changes to the new branch <br/>

git add . <br/>
git commit -m "<commit-message>" <br/>

git restore .                                     # undo unstaged local changes <br/>
git restore hello.c                               # undo unstaged change to specific file <br/>
git restore --staged hello.c                      # undo staged local changes to specific file <br/>

git log main..HEAD <br/>
git log --stat main..HEAD <br/>

git show <commit-hash> <br/>
git show --stat <commit-hash> <br/>

git push <br/>
git push --set-upstream origin <new-branch-name> <br/>
git push --set-upstream azure <new-branch-name> <br/>

git diff --cached                         # to see changes that will be applied on the next commit <br/>
git difftool                              # to view diff side by side | :qa + Enter to quit difftool <br/>
git difftool -- [<file-path>]              # git difftool -- .\infra\gateway-api\main.bicep <br/>

# resetting feature branch to main <br/>
git checkout main <br/>
git fetch origin                          # maket sure you have the latest state of main branch <br/>
git checkout <feature-branch-name> <br/>
git reset --hard origin/main <br/>
git push origin <feature-branch-name> --force             # be cautious when using git reset --hard and git push --force <br/>
                                                          # as they can lead to data loss by discarding commits.  <br/>

