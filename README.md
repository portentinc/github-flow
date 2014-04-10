github-flow
===========

## There is one golden rule. The master branch is **always** deployable

## What is GitHub Flow?

1. Anything in the master branch is deployable
2. To work on something new, create a descriptively named branch off of master (ie: new-sidebar-menu)
3. Commit to that branch locally and regularly push your work to the same named branch on the server
4. When you need feedback or help, or you think the branch is ready for merging, open a pull request
5. After someone else has reviewed and signed off on the feature, you can merge it into master
6. Once it is merged and pushed to ‘master’, you can and should deploy immediately

### Branching

I'm starting with branching because it's the core tenet of using github flow. Everything
goes through branches. Because the master branch is always deployable, the majority of your
pull requests will go into the develop branch.

If you're the only one working on the project there is a strong temptation to just push
to the master branch. Avoid this temptation as it'll sneak up on you when you don't want
to do it. It's happened to me a few times and I've had to revert commits.

Depending on the branch and the work, it's a good idea to delete the branch after you've
merged it to develop. This is especially relevant with smaller fixes and updates. If you've
created a branch to fix some links, there's no real reason to keep that branch. Doing this
ensures that the branch tree isn't cluttered.




### Resources

1. http://scottchacon.com/2011/08/31/github-flow.html
2. https://guides.github.com/overviews/flow/
