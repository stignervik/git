# Git Branch

Create the local branch (if not already created)
```sh
$ git branch feature-branch
```
Push the local branch to the remote repository
```sh
$ git push -u origin feature-branch
```

## Using `git checkout -t`

The `-t` or `--track` option with `git checkout` is used to set up a local branch to track a remote branch. This is useful when you want to create a new local branch that tracks a branch from a remote repository.

### When to Use `git checkout -t`

1. **Creating a Local Branch to Track a Remote Branch**:
   - Use this when you need to work on a remote branch locally.

2. **Setting Up Tracking for Collaboration**:
   - Useful for staying updated with changes made by others on the remote branch.

3. **Simplifying Push and Pull Commands**:
   - Automatically sets up the upstream configuration, so you don’t have to specify the remote branch each time you push or pull.

### Example Usage

Assume you have a remote repository with a branch named `feature-branch`. To create a local branch that tracks this remote branch, use:

```sh
git checkout -t origin/feature-branch
```