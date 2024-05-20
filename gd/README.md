# gd

The `gd` returns a numbered list of local branches. Type a number in and it'll delete that branch.

Output:

```bash
$ gd
1) develop
2) feature/DASH-1-new-feature-1
3) feature/DASH-2-new-feature-2
4) main
#?
```

However it can filter also, so if you type "feature/" it'll bring back only the feature branches.

Output:

```bash
$ gd feature/
1) feature/DASH-1-new-feature-1
2) feature/DASH-2-new-feature-2
#?
```
