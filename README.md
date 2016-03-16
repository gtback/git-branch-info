git-branch-info
===============

Get information about the age and committers on remote branches.

Quickstart
----------
To use, copy this script onto your path and run ```git branch-info```. 

For more user-friendly output, try:

```
git branch-info | sort | cut -f 2-
```

TODO
----
- Handle remotes besides `origin`
- Handle local branches as well as remotes. 