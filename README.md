GitHub-Flow
===========

##### There is one golden rule. The master branch is *always* deployable

## What is GitHub Flow?

1. Anything in the master branch is deployable
2. To work on something new, create a descriptively named branch off of master (ie: new-sidebar-menu)
3. Commit to that branch locally and regularly push your work to the same named branch on the server
4. When you need feedback or help, or you think the branch is ready for merging, open a pull request
5. After someone else has reviewed and signed off on the feature, you can merge it into master
6. Once it is merged and pushed to ‘master’, you can and should deploy immediately

### Branching

I'm starting with branching because it's the core tenet of using github flow. Everything goes through branches. Because the master branch is always deployable, the majority of your pull requests will go into the develop branch.

If you're the only one working on the project there is a strong temptation to just push to the master branch. Avoid this temptation as it'll sneak up on you when you don't want to do it. It's happened to me a few times and I've had to revert commits.

Depending on the branch and the work, it's a good idea to delete the branch after you've merged it to develop. This is especially relevant with smaller fixes and updates. If you've created a branch to fix some links, there's no real reason to keep that branch. Doing this ensures that the branch tree isn't cluttered.

### Commits

It's important to provide a good commit message. Reading through the + & -'s can be time consuming and a pain. A good commit message can reduce the amount of digging around required for both you (at a later date) and for others.



### Resources

1. http://scottchacon.com/2011/08/31/github-flow.html
2. https://guides.github.com/overviews/flow/


### Josh

### Terminal Commands
1. Create the branch on your local machine :
```$ git branch <name_of_your_new_branch>```

2. Push the branch on github :
```$ git push origin <name_of_your_new_branch>```

3. Switch to your new branch :
```$ git checkout <name_of_your_new_branch>```

When you want to commit something in your branch, be sure to be in your branch.

4. You can see all branches created by using
```$ git branch```
Which will show :
```* approval_messages
  master
  master_clean```

5. Add a new remote for your branch :
```$ git remote add <name_of_your_remote> <url>```

6. Push changes from your commit into your branch :
```$ git push origin <name_of_your_remote>```

7. Delete a branch on your local filesytem :
```$ git branch -d <name_of_your_new_branch>```

8. Delete the branch on github :
```$ git push origin :<name_of_your_new_branch>```
