# gfc

The `gfc` returns a numbered list of the branches on that repository (local and remote). Type a number in and it'll checkout that branch, and pull.

Output:

```bash
$ gfc
Please choose the branch you want to checkout:
1) feature/DASH-1-new-feature-1
2) feature/DASH-2-new-feature-2
3) main
#?
```

However it can filter also, so if you type "feature/" it'll bring back only the feature branches.

Output:

```bash
$ gfc feature/
Please choose the branch you want to checkout:
1) feature/DASH-1-new-feature-1
2) feature/DASH-2-new-feature-2
#?
```

## Example aliases

1. `gfcb` = `gfc bugfix/`
2. `gfcd` = `git develop`
3. `gfcf` = `gfc feature/`
4. `gfch` = `gfc hotfix/`
5. `gfcm` = `gfc main master`
6. `gfcr` = `gfc release/`
7. `gfct` = `gfc task/`
