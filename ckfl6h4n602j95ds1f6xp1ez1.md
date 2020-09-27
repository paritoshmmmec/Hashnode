## Merge forked branch from the upstream branch in git

If you are working on an open-source, you might need to create a fork out of the project. Over a period of time, you might diverge from the base branch of the project and might want to sync it, following the git command may help you to do so:


- Fetch upstream from the original repo, it will bring all tags and change tracker 

``` 
git fetch upstream

``` 
- Check out the master/main branch in the forked repository and merge from the upstream master/main branch as follows 

```
git merge upstream/master

```

That is it.
Happy gitting

Edit: Title update to make it clear