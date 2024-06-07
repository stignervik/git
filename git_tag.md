# Git tag
Git tags are used to mark specific points in a repository’s history as important, typically for releases. Tags are like bookmarks that help identify significant milestones, making it easy to reference and manage versions of your project. This aids in release management, version tracking, and ensuring consistency across deployments.

For an annotated tag (recommended for releases):
```sh
$ git tag -a v1.0 -m "Release version 1.0"
```
Push the tag to the remote repository:
```sh
$ git push origin v1.0
```
List all tags (to verify):
```sh
$ git tag
```
List all tags with descriptions (annotations)
```sh
$ git tag -n
```

Delete a tag (if needed) 
Locally:
```sh
git tag -d v1.0
```
Remotely:
```sh
git push origin --delete tag v1.0
```