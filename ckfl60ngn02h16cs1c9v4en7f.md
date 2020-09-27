## Undo git mistakes

We all make mistake when interacting with git, and sometimes we want to undo stuff which can help us. Actually, this blog aimed at me to keep a collection of commands which I use regularly (haha). Here are some scenarios we will be covering:

**Scenarios 1: Checked into main/master local branch **

Problem: I always wanted my local main/master branch to be sync with the remote main/master branch. Although some time due to I commit to main/master. This frustrates me a lot. 

Solution: 

- Create a new branch to save code so we don't want to lose the work

```
  git checkout -b <branch_name> 

```

```
  git push origin  <branch_name>
 
```

-  Next is the checkout main/master and run the following command. Be care full there is no revert here

```
  git reset --hard 
    
``` 

**Scenarios 2: Modified file(s) which you did not want to change  **

Problem: Some time working on a branch, some file(s) I touched which were not required. This makes the code reviewer's job a bit hard.   

Solution: 

-  Run the following command will reset a single file from the origin master or main branch. Please note there is a space between `--` and file path. The file path is relative to the root folder of the project.

```
 git checkout origin/master  --  file-path
    
``` 

The relative file path from the root may look like `src/AutofacDependencyConfigurator.cs`

Happy gitting