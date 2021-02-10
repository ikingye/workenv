---
weight: 10
title: "编程"
bookCollapseSection: true
---

# 编程

## multipass

[canonical/multipass](https://github.com/canonical/multipass) ![Github stars](https://img.shields.io/github/stars/canonical/multipass.svg) ![Language](https://img.shields.io/github/languages/top/canonical/multipass.svg) ![Last Tag](https://img.shields.io/github/v/tag/canonical/multipass.svg?sort=semver) ![Last commit](https://img.shields.io/github/last-commit/canonical/multipass.svg)

```shell
# 创建一个 VM, 1GB 内存和 5GB 磁盘
multipass launch --name myvm --mem 1G --disk 5G

# 为 VM 启动一个 shell
multipass shell myvm

# 挂载
multipass mount ~/code myvm:/home/ubuntu/yewang/code
```

---

## Tmux

[gpakosz/.tmux](https://github.com/gpakosz/.tmux) ![Github stars](https://img.shields.io/github/stars/gpakosz/.tmux.svg) ![Language](https://img.shields.io/github/languages/top/gpakosz/.tmux.svg) ![Last Tag](https://img.shields.io/github/v/tag/gpakosz/.tmux.svg?sort=semver) ![Last commit](https://img.shields.io/github/last-commit/gpakosz/.tmux.svg)

参考：

- [手把手教你使用终端复用神器 Tmux，丢掉鼠标不是梦 [视频]](https://zhuanlan.zhihu.com/p/43687973)
- [让你的 tmux 起死回生！[视频]](https://zhuanlan.zhihu.com/p/259640277)

---

---

## 网络

### nps

[ehang-io/nps](https://github.com/ehang-io/nps) ![Github stars](https://img.shields.io/github/stars/ehang-io/nps.svg) ![Language](https://img.shields.io/github/languages/top/ehang-io/nps.svg) ![Last Tag](https://img.shields.io/github/v/tag/ehang-io/nps.svg?sort=semver) ![Last commit](https://img.shields.io/github/last-commit/ehang-io/nps.svg)

server

```shell
# 安装
sudo ./nps install

# 启动
sudo nps start

# 访问 web
http://localhost:8080/
# 账户密码
# admin/123

# 日志
sudo tail -f /var/log/nps.log
```

client

[下载 client](https://github.com/ehang-io/nps/releases)

```shell
./npc -server=192.168.64.1:8024 -vkey=qlati48ufop46lln -type=tcp
```

---

### goproxy

[snail007/goproxy](https://github.com/snail007/goproxy) ![Github stars](https://img.shields.io/github/stars/snail007/goproxy.svg) ![Language](https://img.shields.io/github/languages/top/snail007/goproxy.svg) ![Last Tag](https://img.shields.io/github/v/tag/snail007/goproxy.svg?sort=semver) ![Last commit](https://img.shields.io/github/last-commit/snail007/goproxy.svg)

Proxy 是 golang 实现的高性能 http,https,websocket,tcp,socks5 代理服务器，支持内网穿透，链式代理，通讯加密，智能 HTTP,SOCKS5 代理，黑白名单，限速，限流量，限连接数，跨平台，KCP 支持，认证 API。
