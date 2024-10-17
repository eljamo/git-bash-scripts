# gd

The `gd` returns a numbered list of local branches. Type a number in and it'll delete that branch.

Output:

```bash
$ gd
Please choose the branch you want to delete locally (this will not delete the remote branch):
1) feature/DASH-1-new-feature-1
2) feature/DASH-2-new-feature-2
3) main
4) Cancel
#?
```

However it can filter also, so if you type "feature/" it'll bring back only the feature branches.

Output:

```bash
$ gd feature/
Please choose the branch you want to delete locally (this will not delete the remote branch):
1) feature/DASH-1-new-feature-1
2) feature/DASH-2-new-feature-2
3) Cancel
#?
```

You can also switch the branch search mode from `OR` to `AND`

```bash
$ gd --branch_search_mode=AND feature/ DASH-1
Please choose the branch you want to delete locally (this will not delete the remote branch):
1) feature/DASH-1-new-feature-1
2) Cancel
#?
```
