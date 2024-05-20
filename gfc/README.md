# gfc

The `gfc` returns a numbered list of the branches on that repository (local and remote). Type a number in and it'll checkout that branch, and pull.

Output:

```
/a/m/h/d/c/d/dashboard $ gfc
1) develop
2) feature/DASH-1-new-feature-1
3) feature/DASH-2-new-feature-2
4) main
#? 3
```

However it can filter also, so if you type "feature/" it'll bring back only the feature branches.

Output:

```
/a/m/h/d/c/d/dashboard $ gfc feature/
1) feature/DASH-1-new-feature-1
2) feature/DASH-2-new-feature-2
#?
```

## Aliases I Use

```
1) gfcb = gfc bugfix/
2) gfcd = git develop
3) gfcf = gfc feature/
4) gfch = gfc hotfix/
5) gfcm = gfc main master
6) gfcr = gfc release/
```
