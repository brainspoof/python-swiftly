---
description: Now, just one liner git push
---

# Git push

While working with a project, most of the time, you just add \* to git, then commit it, and then push. Well, why not all in the same command

```batch
swiftly push "commit message"
```

This is works even better with lesser merge conflicts as every time you init a swiftly project, we check to make sure that you are up-to-date with the latest changes in the remote git repo. This increases the likelihood of a successful merge without any conflicts.

Incase of conflicts, you can always use git cli to fix the conflicts.
