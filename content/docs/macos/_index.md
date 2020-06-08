---
weight: 10
title: "MacOS"
---

# MacOS

## 虚拟机

### [canonical/multipass](https://github.com/canonical/multipass) ![Github stars](https://img.shields.io/github/stars/canonical/multipass.svg)

```shell
# 创建一个 VM, 1GB 内存和 5GB 磁盘
multipass launch --name myvm --mem 1G --disk 5G

# 为 VM 启动一个 shell
multipass shell myvm
```
