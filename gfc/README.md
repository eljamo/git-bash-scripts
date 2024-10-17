# gfc

The `gfc` returns a numbered list of the branches on that repository (local and remote). Type a number in and it'll checkout that branch, and pull.

Output:

```bash
$ gfc
Please choose the branch you want to checkout:
1) feature/DASH-1-new-feature-1
2) feature/DASH-2-new-feature-2
3) main
4) Cancel
#?
```

However it can filter also, so if you type "feature/" it'll bring back only the feature branches.

Output:

```bash
$ gfc feature/
Please choose the branch you want to checkout:
1) feature/DASH-1-new-feature-1
2) feature/DASH-2-new-feature-2
3) Cancel
#?
```

You can also switch the branch search mode from `OR` to `AND`

Output:

```bash
$ gfc --branch_search_mode=AND feature/ DASH-1
Please choose the branch you want to checkout:
1) feature/DASH-1-new-feature-1
2) Cancel
#?
```

## Example aliases

1. `gfcb` = `gfc --branch_search_mode=AND bugfix/ "$@"`
2. `gfcd` = `gfc develop`
3. `gfcf` = `gfc --branch_search_mode=AND feature/ "$@"`
4. `gfch` = `gfc --branch_search_mode=AND hotfix/ "$@"`
5. `gfcm` = `gfc main master`
6. `gfcr` = `gfc --branch_search_mode=AND release/ "$@"`
7. `gfct` = `gfc --branch_search_mode=AND task/ "$@"`
