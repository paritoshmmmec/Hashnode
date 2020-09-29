## Frequent git commands

** Add all uncommitted file into staged area **

```
git add .

```

** Commit staged files to git permanent area  **

```
git commit -m "feat(server) : adding new functionality"

```


** Clone a repository **

```
git clone <http or git url>

```


** Check the history and commit id **

```
git log

```

** Check the status of current branch **

```
git status

```

** Check out a branch **

```
git checkout -b <branch-name>

```

** Merge from remote branch **

```
git fetch && git merge origin/main

```

** Checkout colleague branch **

```
git fetch && git checkout <collegau-name>

```

** Merge from colleague branch**

```
git pull 

```

** Revert the particular commit **

```
git revert <commitid>

```

Note: All main branch referred above origin/master or origin/main or upstream/<main branch>.  