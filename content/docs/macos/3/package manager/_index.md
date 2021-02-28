---
weight: 15
title: "包管理工具"
bookCollapseSection: true
---

# 包管理工具

## Linux

### Ubuntu

#### apt

```shell
sudo apt install

# download .deb package
sudo dpkg -i fd_8.0.0_amd64.deb  # adapt version number and architecture
```

### Debian

#### apt-get

```shell
sudo apt-get install
```

### Fedora

#### dnf

```shell
dnf install
```

##### dnf copr

```shell
dnf copr enable keefle/fd
dnf install fd
```

### Alpine Linux

#### apk

```shell
apk add
```

### Arch Linux

#### pacman

```shell
pacman -S
```

### Gentoo Linux

#### emerge

```shell
emerge -av
```

### openSUSE Linux

#### zypper

```shell
zypper in
```

### Void Linux

#### xbps-install

```shell
xbps-install -S
```

### FreeBSD

#### pkg

```
pkg install
```

---

## Mac

### Homebrew

### MacPorts

---

## Windows

### [Scoop](http://scoop.sh/)

### [Chocolatey](https://chocolatey.org/)

## 其他

### NixOS / via Nix

#### [Nix package manager](https://nixos.org/nix/)

```shell
nix-env -i
```

### Node.js

#### NPM

```shell
# On linux and macOS
npm install -g
```

### Rust

#### cargo

```
cargo install
```
