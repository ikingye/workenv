---
weight: 10
title: "MacOS"
bookCollapseSection: true
---

# MacOS

## 虚拟机

### [canonical/multipass](https://github.com/canonical/multipass) ![Github stars](https://img.shields.io/github/stars/canonical/multipass.svg)

```shell
# 创建一个 VM, 1GB 内存和 5GB 磁盘
multipass launch --name myvm --mem 1G --disk 5G

# 为 VM 启动一个 shell
multipass shell myvm

# 挂载
multipass mount ~/code myvm:/home/ubuntu/yewang/code
```

---

## 网络

### 代理

#### [ehang-io/nps](https://github.com/ehang-io/nps) ![Github stars](https://img.shields.io/github/stars/ehang-io/nps.svg)

##### server

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

##### client

[下载 client](https://github.com/ehang-io/nps/releases)

```shell
./npc -server=192.168.64.1:8024 -vkey=qlati48ufop46lln -type=tcp
```

---

#### [snail007/goproxy](https://github.com/snail007/goproxy) ![Github stars](https://img.shields.io/github/stars/snail007/goproxy.svg)

---

### 抓包

### 发包
