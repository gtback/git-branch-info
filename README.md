git-branch-info
===============

Get information about the age and committers on remote branches.

GitHub, GitLab, Bitbucket all show the number of commits "ahead" and "behind",
but this adds the ability to show who has committed to each branch.

Quick Start
-----------

To use, copy this script onto your path and run ```git branch-info```.

For more user-friendly output, try:

```shell
git branch-info | sort | cut -f 2-
```

Output
------

Example output from running on the [Flask](https://github.com/mitsuhiko/flask)
repository:

```text
6 years ago      0.3-maintenance         armin.ronacher (5)
6 years ago      0.5-maintenance         armin.ronacher (4)
6 years ago      new-logging     armin.ronacher (6)
5 years ago      new-modules     armin.ronacher (7) jweber (1)
5 years ago      0.6-maintenance         armin.ronacher (11) lee (1)
5 years ago      appdispatch-docs
4 years, 10 months ago   new-request-dispatching
4 years, 8 months ago    0.7-maintenance         armin.ronacher (14)
3 years, 10 months ago   feature/remove-jsonp    armin.ronacher (1)
3 years, 9 months ago    0.8-maintenance
3 years, 7 months ago    json-sessions
2 years, 10 months ago   sprint-branch
1 year, 5 months ago     flask_deployment_docs
10 months ago    ext-deprecation         dasdasich (5) jeff (2) markus (1)
7 weeks ago      0.10-maintenance        nadav.geva4 (1) davidism (1)
2 days ago       master
```

TODO
----

- Handle remotes besides `origin`
- Handle local branches as well as remotes.
- Show total number of commits ahead and behind master (or current branch)

Contributing
------------

Issues, comments and merge requests welcome!
