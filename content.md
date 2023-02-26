## Content

### What are the differences between the push, fetch, and pull git commands?

#### `git push` 

The `git push` command sends changes from your local branch to a tracking branch in a connected remote repository.

The changes from this command match the remote branch with your local branch. If your local branch is missing commits from the remote branch, the push fails. 

If your local branch is missing commits, run `git pull` or `git fetch` and `git merge` to synchronize with your remote branch.

#### `git fetch` 

The `git fetch` command gets changes from a remote repository into your tracking branch. This command does not change your local branch. 

To merge your tracking branch changes into your local branch, run `git merge origin/master`.

#### `git pull` 

will get changes from a remote branch into your tracking branch and merge them into a local branch

Often `git push` and `git pull` are described as equivalent. This isn't entirely correct, since under the hood `git pull` does two things. 

`git pull` simply does a `git fetch` followed immediately by `git merge`. This is often what we desire to do, but some people prefer to use git fetch followed by git merge to make sure they understand the changes they are merging into their branch before the merge happens.




