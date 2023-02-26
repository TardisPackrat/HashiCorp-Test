## Content

### What are the differences between the push, fetch, and pull git commands?


| Command | Description |
| ----------- | ----------- |
| `git push` | The `git push` command sends changes from your local branch to a tracking branch in a connected remote repository.<br><br>The changes from this command match the remote branch with your local branch. If your local branch is missing commits from the remote branch, the push fails. <br><br>If your local branch is missing commits, run `git pull` or `git fetch` and `git merge` to synchronize with your remote branch. |
| `git fetch` | The `git fetch` command gets changes from a remote repository into your tracking branch. This command does not change your local branch. <br><br>To merge your tracking branch changes into your local branch, run `git merge origin`. |
| `git pull` | The `git pull` command gets changes from a remote branch into your tracking branch and merges them into your local branch. This is identical to running `git fetch` followed by `git merge`. <br><br>To review the changes you are making prior to merging, use the `git fetch` command. After you've reviewed your changes, run the `git merge` command to merge them. |

