## Releasing a new version

1. Sync the fork's main branch with its upstream.
2. Checkout the commit revision associated with the release.
3. Make any needed changes to the repository (it's possible the previous patch just needs to be applied).
4. Run `git diff > rustls+{sem_ver}.patch`.
5. Commit the changes (including the patch file).
6. Create a new tag for the release and push it.
7. Copy the patch file over to the master branch and push it.

## Applying the patch

Simply run `git apply rustls+{sem_ver}.patch`
