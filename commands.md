1. **git init** - Initializes a new, empty Git repository in the current directory. This command creates a new subdirectory named `.git` that contains all of your necessary repository files.
```sh
git init
```

2. **git clone** - Creates a local copy of a remote repository. This command creates a copy of an existing repository in a new directory.
```sh
git clone https://github.com/username/repository.git
```

3. **git staus** - Displays the state of the working directory and the staging area. This command shows which changes have been staged, which haven’t, and which files aren’t being tracked by Git.
```sh
git status
```

4. **git add** - Stages a specific file or all changes in the directory (with `.`) for the next commit. The first command stages a specific file, and the second stages all changes in the working directory.
```sh
git add filename
git add .
```

5. **git commit** - Commits staged changes with a descriptive message. This command commits the staged snapshot with a message describing the changes.
```sh
git commit -m "Commit message"
```

6. **git log** - Shows the commit logs. This command displays the commit history with details of each commit.
```sh
git log
```

7. **git branch** - Lists, creates, or deletes branches. The first command lists all branches, and the second command creates a new branch.
```sh
git branch
git branch new-branch
```

8. **git checkout** - Switches to specific branch. Creates and switches to new-branch.
```sh
git checkout main
git checkout -b new-branch
```

9. **git merge** - This command merges the specified branch into the current branch.
```sh
git merge branch-name
```

10. **git remote** - Manages set of tracked repositories. The first command shows the URLs that a repository is tracking, and the second command adds a new remote repository.
```sh
git remote -v
git remote add origin https://github.com/username/repository.git
```

11. **git pull** - Fetches from and integrates with another repository or a local branch. This command fetches and merges changes from the remote repository's main branch into the current branch.
```sh
git pull origin main
```

12. **git push** - Updates remote refs along with associated objects. This command pushes the local branch `main` to the remote repository named `origin`.
```sh
git push origin main
```

13. **git diff** - Shows changes between the working directory and the staging area. To compare branches, use second command.
```sh
git diff
git diff branch1 branch2
```

14. **git stash** - Stashes changes in the working directory. The first command stashes the current changes, and the second applies the stashed changes back to the working directory.
```sh
git stash
git stash pop
```

15. **git rebase** - Replays changes from the current branch onto the latest main branch commits.
```sh
git rebase main
```

16. **git reset** - Resets current HEAD to the specified state(Removes `filename.txt` from the staging area). The `--soft` flag undoes the last commit but keeps changes staged, while `--hard` discards them completely.
```sh
git reset filename.txt
git reset --soft HEAD~1
git reset --hard HEAD~1
```

17. **git fetch** - Downloads objects and refs from another repository. This command fetches updates from the remote repository named origin without merging them into the current branch.
```sh
git fetch origin
```

18. **git cherry-pick** - Applies the changes introduced by some existing commits. This command applies the changes from the commit with the specified hash to the current branch.
```sh
git cherry-pick commit-hash 
```

19. **git revert** - Reverts a commit by creating a new commit that undoes the changes. This command creates a new commit that reverses the changes made by the specified commit.
```sh
git revert commit-hash
```

20. **git tag** - Tags a commit with a version number (e.g., v1.0) and pushes it to the remote repository. The first command lists all tags, the second creates an annotated tag `v1.0` with a message, and the third deletes the tag `v1.0`.
```sh
git tag
git tag -a v1.0 -m "Version 1.0"
git tag -d v1.0
```

21. **git config** - Sets configuration options for Git installation. These commands set the global username and email address for commits.
```sh
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

22. **git show** - Shows the details of a specific commit, identified by its hash.
```sh
git show <commit-hash>
```

23. **git mv** - Moves or renames a file, a directory, or a symlink. This command renames a file and stages the change for commit.
```sh
git mv old-filename new-filename
```

24. **git rm** - Removes files from the working tree and from the index. This command deletes a file from the working directory and stages the change for commit.
```sh
git rm filename
```

25. **git clean** - Removes untracked files from the working directory. The first command removes untracked files, and the second removes untracked files and directories.
```sh
git clean -f
git clean -fd
```