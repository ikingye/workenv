---
weight: 10
title: "ssh"
bookCollapseSection: true
---

# ssh

## ssh-keygen

## 代理

```shell
ssh -o ProxyCommand='socat - SOCKS4A:myproxy:%h:%p,socksuser=nobody' user@host

# SOCKS5
ssh -o ProxyCommand='socat - "SOCKS5:%h:%p|tcp:myproxy:1080"' user@host

# http
ssh -o ProxyCommand='socat - "PROXY:%h:%p|tcp:myproxy:80"' user@host
```

参考：

- [Connecting to host by SSH client in Linux by proxy](https://unix.stackexchange.com/questions/68826/connecting-to-host-by-ssh-client-in-linux-by-proxy)
