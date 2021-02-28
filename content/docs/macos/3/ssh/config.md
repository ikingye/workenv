---
weight: 10
title: "config"
bookCollapseSection: true
---

# config

## my config

```shell
################ vps ################
Host bcc
    HostName 106.13.4.39
    User root
    IdentityFile ~/.ssh/id_rsa

Host vultr
    HostName 149.28.142.246
    User root
    IdentityFile ~/.ssh/id_rsa

################ baidu ################
Host baidu
    HostName relay.baidu-int.com
    User yewang

################ git ################
Host github
    HostName github.com
    User git
    IdentityFile ~/.ssh/id_rsa
    ProxyCommand nc -v -x 127.0.0.1:1081 %h %p
Host gitlab
    HostName gitlab.com
    User git
    IdentityFile ~/.ssh/id_rsa
    ProxyCommand nc -v -x 127.0.0.1:1081 %h %p
Host bitbucket
    HostName bitbucket.org
    User git
    IdentityFile ~/.ssh/id_rsa
    ProxyCommand nc -v -x 127.0.0.1:1081 %h %p
Host gitcafe
    HostName e.coding.net
    User git
    IdentityFile ~/.ssh/id_rsa
Host gitee
    HostName gitee.com
    User git
    IdentityFile ~/.ssh/id_rsa

################ others ################
Host *
    # 复用之前已经建立的连接
    ControlMaster auto
    # 在最后一个连接关闭之后也不真正的关掉连接
    ControlPersist yes
    # 指定了这个连接的 socket 保存的路径
    ControlPath ~/.ssh/connection-%r@%h:%p
    # 心跳
    ServerAliveInterval 60
    # ServerAliveCountMax 20
    # ForwardAgent yes
    # KexAlgorithms +diffie-hellman-group1-sha1
    # PreferredAuthentications publickey
    # TCPKeepAlive no
    # Compression yes

    # 走 HTTP 代理
    # ProxyCommand socat - PROXY:127.0.0.1:%h:%p,proxyport=8081
    # 走 socks5 代理（如 Shadowsocks）
    # ProxyCommand nc -v -x 127.0.0.1:1080 %h %p
```
