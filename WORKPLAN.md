# Work split (2 partners)

## Moderator requirement
Submit your GitHub Profile README output + the evaluation form.
Each partner finishes their own file in `profiles/`, then copies it into
their own profile repo (a repo named exactly your-username, with README.md).

## Setup (Sandy)
    git init
    git add .
    git commit -m "Initial commit: project skeleton"
    git branch -M main
    git remote add origin <repo-url>
    git push -u origin main
Partner: `git clone <repo-url>` (Sandy adds partner as collaborator)

## Sandy - branch `feature/profile-sandy`
    git switch -c feature/profile-sandy
1. Fill `profiles/sandy.md` + card A in index.html -> commit
2. Finish README                                   -> commit
    git push -u origin feature/profile-sandy

## Partner - branch `feature/profile-partner`
    git switch -c feature/profile-partner
1. Fill `profiles/partner.md` + card B in index.html -> commit
2. Improve style.css                                 -> commit
    git push -u origin feature/profile-partner

## Merge (together)
    git switch main
    git pull
    git merge feature/profile-sandy
    git merge feature/profile-partner
    git push
Conflict in index.html? Keep both sections, save, `git add . && git commit`.

## Quest checklist
- [ ] Start: git init / clone
- [ ] Commit: initial + at least 2 more (we get 1 + 2 each = 5)
- [ ] Branch: feature branch
- [ ] Improve: commit on that branch
- [ ] Merge: both branches into main
- [ ] Publish: push, then `git log --oneline --graph --all`

## Before you present (60-90 sec: built / how / learned)
- [ ] Repo link ready
- [ ] README readable
- [ ] Commit history visible
- [ ] Features merged
- [ ] No passwords, tokens or secrets committed
