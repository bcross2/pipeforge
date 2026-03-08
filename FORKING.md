# Forking PipeForge

PipeForge lives at `https://github.com/bcross2/pipeforge`.

## Fork on GitHub

1. Sign in to GitHub with the account or organization that should own the fork.
2. Open `https://github.com/bcross2/pipeforge`.
3. Click `Fork` in the top-right corner.
4. Choose the destination owner and create the fork.
5. Clone your fork:

```bash
git clone git@github.com:YOUR-ACCOUNT/pipeforge.git
cd pipeforge
```

## Fork with GitHub CLI

```bash
gh repo fork bcross2/pipeforge --clone
```

If you want the fork under an organization:

```bash
gh repo fork bcross2/pipeforge --org YOUR-ORG --clone
```

## Keep Your Fork Up To Date

If you cloned from your fork, add the original repo as `upstream`:

```bash
git remote add upstream git@github.com:bcross2/pipeforge.git
git fetch upstream
git merge upstream/master
```

If the default branch is `main` instead of `master`, replace the last command with:

```bash
git merge upstream/main
```

## Important Note

GitHub will not create a fork back into the same owner namespace as the original repo. Because the source repo is already owned by `bcross2`, an actual fork must go to a different GitHub user or organization.
