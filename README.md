# WEEK-2
## Version Control

It is an important tool that helps track changes to code orother creative projects.<br/>  It gives software engineering teams complete visibility to the code history and a single source of documentation  for all folders, files and messages.

## Difference between git and github
|             GIT                 |         GITHUB                 |
|     :-----------------          |     ---------------:           |                   
| A software tool                 | A web-based service.           |
| A distributed version control system | A repository hosting and collaboration platform.|
| Primarily used through a command-line interface.| Provides a web-based graphical interface |
|Maintained by the open-source community. | Maintained by Microsoft|
|Focuses on version control and change tracking. | Focuses on coode holsting and collaboration. |

## Github alternatives
- Gogs
* AWS CodeCommit
+ OneDev

## Difference between git fetch and git pull

+ Git pull is a command that performs git fetch follwed by git merge or git rebase. While git fetch does not affect the local repository, it automatically synchronozes changes from the remote repository with the local repository.

- During git pull, the working directory is updated directly but for git fetch the repository data is updated in the .git directory.

* There is a possibility of a merge conflict in git fetch, while merge  conflicts are possible if the remote and local repositories have done changes at the same time using git pull.

## git re-base and its command 

This moves or combines a sequence of commits to a new base commit. It is often used to keep a clean, linear project history. Its command include:
1. Run on the branch you want to rebase. `git checkout <feature-branch>`
2. Update the local base branch with the latest changes from the remote. `git pull origin <base-branch-name>`
3. Reapply your current branch commits on top of the <base-branch-name>. `git rebase <base-branch-name>`

## git cherry-pick and its command

This allows youto apply a specific commit from one branch onto another wihtou merging the entire branch. Usually the command automatically creates a sequence of commits.
* Source the branch to find the SHA of desired commit. `git log`
+ Switch to the bracnh you want the changes to be made in. `git checkout <target-branch-name>`
- Run cherry-pick by creating new commit on your current branch with the same changes as the original. `git cherry-pick <commit-hash>`