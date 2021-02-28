---
weight: 15
title: "homebrew"
bookCollapseSection: true
---

# Homebrew

## tap

brew tap 可以为 brew 的软件的 跟踪，更新，安装添加更多的的 tap formulae

如果你在核心仓库没有找到你需要的软件，那么你就需要安装第三方的仓库去安装你需要的软件

tap 命令的仓库源默认来至于 Github，但是这个命令也不限制于这一个地方

### brew tap

没有参数会自动更新已经存在的 tap 并列出当前已经 tapped 的仓库

```shell
# URL 默认是 https://github.com/user/homebrew-repo
brew tap <user>/<repo>
brew tap <user>/<homebrew-repo>

# URL 可以是任何位置，任何协议
brew tap <user>/<repo> URL
```

homebrew/core 默认是最高优先级

可以使用 brew tap-pin username/repo 使这个仓库优先级高于 core

使用 brew-tap-unpin username/repo 取消

当你使用 brew install foo 这个命令时，brew 将按照下面的顺序去查找哪个 formula(tap) 将被使用:

1. pinned taps
2. core formulae
3. other taps

---

## 镜像加速

### [清华大学镜像](https://mirror.tuna.tsinghua.edu.cn/help/homebrew/)

替换现有上游

```shell
# brew 程序本身，Homebrew/Linuxbrew 相同
git -C "$(brew --repo)" remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/brew.git

# 以下针对 mac OS 系统上的 Homebrew
git -C "$(brew --repo homebrew/core)" remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-core.git
git -C "$(brew --repo homebrew/cask)" remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-cask.git
git -C "$(brew --repo homebrew/cask-fonts)" remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-cask-fonts.git
git -C "$(brew --repo homebrew/cask-drivers)" remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-cask-drivers.git

# 以下针对 Linux 系统上的 Linuxbrew
git -C "$(brew --repo homebrew/core)" remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/linuxbrew-core.git

# 更换后测试工作是否正常
brew update
```

---

## 参考

- [Homebrew 和 Fink、MacPort 相比有什么优势？](https://www.zhihu.com/question/19862108)
- [解决 Homebrew 下载更新极慢的问题](https://www.raydbg.com/2019/Homebrew-Update-Slow/)
