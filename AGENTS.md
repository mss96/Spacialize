# Git workflow

This repository uses Git and GitHub.

Remote
- origin git@github-personalmss96Spacialize.git
- default branch main

For every completed task that changes repository files

1. Review `git status` and `git diff`.
2. Never commit secrets, credentials, `.env` files, generated dependencies, or files ignored by `.gitignore`.
3. Stage only the files relevant to the task.
4. Run any relevant validation or tests before committing.
5. Create a Git commit with a short, descriptive commit message.
6. Push the commit to `origin` on the current branch.
7. Run `git status` after pushing and verify that the working tree is clean.
8. Report the commit hash and branch that were pushed.

Do not amend, rewrite, force-push, or delete existing Git history unless explicitly requested.
Do not push if validationtests fail; report the problem instead.