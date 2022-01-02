# 10 Day-to-day Useful Commands

1. git init

Create an empty Git repository or reinitialize an existing one
```
git init
```

> Tip: In an existing repository it is safe to run git init as it would not override anything that is already there.

2. git clone

Clone a repository into a new directory
```
// Clone via HTTPS URL:
git clone <https url>

// Clone via SSH URL:
git clone <ssh url>

// Clone via Github CLI:
gh repo clone <project-name>
```
Last but not least, simply download the zip or via Github Desktop App.

3. git branch

Branches play a vital role in the development world by allowing parallel development work
```
// To create a new branch:
git branch <branch_name>

// To list existing branch(es):
git branch or git branch --list // list local branches
git branch -r // list remote branches
git branch -a // list local and remote branches

// To delete branch(es):
git branch -d <branch_name> // delete branch locally
git branch -D <branch_name> // forcefully delete branch locally
git push origin --delete <branch_name> // delete branch remotely

// Multiple branches can be deleted in one go:
git branch -D <branch_1> <branch_2> ... <branch_n>
```

4. git checkout

Creating a new branch or switching to an existing local or remote branch
```
// Create branch:
git checkout -b <branch_name>

// Furthermore, if we would like to switch to an existing local or remote branch, we can do so by:
git checkout <branch_name>
```

5. git add

Adding file contents to the index
```
// Adding a single file:
git add <file>

// Adding all the files:
git add
.or
git add -A
```
> IMP: git add command does not save the changes until they are committed.

6. git diff

Allows the developer to view the unstaged or staged changes

```
// To view unstaged changes:
git diff

// To view staged changes:
git diff --staged
```

7. git stash

Stash the changes in a dirty working directory away
```
// Simply stash changes:
git stash

// To view list of stash:
git stash list

// To inspect a stash:
git stash show

// To restore a stash:
git stash apply
```
> Note: Calling git stash without any arguments is equivalent to git stash push

8. git status

Show status of the current working tree
```git status```

9. git commit

Commit the change(s) to a repository
```git commit -m "meaningful message"```

> For best practice, please follow [Angular Commit Message](https://github.com/angular/angular/blob/master/CONTRIBUTING.md)

10. git push

Update remote refs with the local commits
```git push -u origin <branch_name>```

> Note: This would also push the branch to remote if it is newly created.
