**git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
git config --global init.defaultBranch main**


git init                           # Initialize a new local Git repository
git clone <url>                    # Download an existing repository from remote



git status                         # View changed, untracked, or staged files
git diff                           # Show unstaged changes line-by-line
git add <filename>                 # Stage specific file for next commit
git add .                          # Stage ALL changed & new files
git commit -m "Your descriptive message"   # Commit staged changes
git commit -am "Short message"     # Stage tracked modified files AND commit in one step



git branch                         # List local branches (* shows current)
git branch <branch-name>          # Create a new branch
git switch <branch-name>          # Switch to a branch (or `git checkout <branch>`)
git switch -c <branch-name>       # Create AND switch to a new branch
git merge <branch-name>           # Merge specified branch into current branch
git branch -d <branch-name>       # Delete local branch (safely)


git remote add origin <url>        # Connect local repo to remote URL
git fetch                          # Download remote updates (does not alter local files)
git pull                           # Download and merge updates into current branch
git push origin <branch-name>      # Push branch to remote
git push -u origin <branch-name>   # Push AND set upstream default tracking


git log                            # View commit history
git log --oneline --graph --all    # Compact visual log tree of all branches
git show <commit-hash>             # View details and diff of a specific commit
git blame <filename>              # Show line-by-line author details for a file


git restore <filename>             # Discard local unstaged changes to a file
git restore --staged <filename>    # Unstage a file (keep local edits)
git commit --amend -m "New text"   # Modify the last commit message or add staged files to it
git stash                          # Temporarily stash uncommitted changes away
git stash pop                      # Re-apply stashed changes and delete from stash list
git reset --soft HEAD~1            # Undo last commit, but KEEP changes staged
git reset --hard HEAD~1            # Nuke last commit AND all uncommitted changes (destructive!)



