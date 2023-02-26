## Content

### What are the differences between the push, fetch, and pull git commands?

#### `git push` 

The `git push` command sends changes from your local branch to a tracking branch in a connected remote repository.

The changes from this command match the remote branch with your local branch. If your local branch is missing commits from the remote branch, the push fails. 

If your local branch is missing commits, run `git pull` or `git fetch` and `git merge` to synchronize with your remote branch.

#### `git fetch` 

get changes from a remote repo into your tracking branch
`git fetch` again takes our current branch, and checks to see if there is a tracking branch. If so, it looks for changes in the remote branch, and pulls them into the tracking branch. It does not change your local branch. To do that, you'll need to do `git merge origin/master` (for the "master" branch) to merge those changes into your branch - probably also called "master".


#### `git pull` 

will get changes from a remote branch into your tracking branch and merge them into a local branch

Often `git push` and `git pull` are described as equivalent. This isn't entirely correct, since under the hood `git pull` does two things. 

`git pull` simply does a `git fetch` followed immediately by `git merge`. This is often what we desire to do, but some people prefer to use git fetch followed by git merge to make sure they understand the changes they are merging into their branch before the merge happens.




