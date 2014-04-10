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

### Pull Requests

Pull Requests are the other major thing to grasp when using GitHub Flow. The pull request is where you can inspect incoming code, discuss what's going on in the pull request with others, and test out new things.

* Not all pull requests have to be merged. If you have an experimental piece of code that you want to test out, feel free to leave it as a pull request until all the tests are complete.
* You don't have to have code in a pull request. You can use a pull request to spark a discussion with screenshots and @mentions. Anyone with access to the repo can view pull requests and comment on them.
* You can keep working on code even after you've done a pull request. If you make a pull request and then realize you forgot to add a certain font-size for example, you can just push that change up and it will be reflected.
* You can comment on individual lines of code. Under the *Files changed* tab you see a list of line number commits. If you hover over the line, you'll see a little blue message icon pop up on the left hand side.

### Resources

1. http://scottchacon.com/2011/08/31/github-flow.html
2. https://guides.github.com/overviews/flow/
