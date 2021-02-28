---
weight: 10
title: "git config"
bookCollapseSection: true
---

# git config

## config 权限

问题： `Bad owner or permissions on ~/.ssh/config`

解决：

```
chown $USER ~/.ssh/config
chmod 644 ~/.ssh/config
```
