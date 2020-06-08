---
weight: 30
title: "VPS"
---

# VPS

## zsh

### [oh-my-zsh](https://ohmyz.sh/)

```shell
https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh
```

### 提示符

```shell
export PROMPT='%{$fg[magenta]%}%(?..%?%1v)%n@%{$fg[green]%}%M:%{$fg[cyan]%}%c%{$reset_color%} $(git_prompt_info)'
```

### 设置默认 shell

```shell
sudo chsh -s /usr/bin/zsh
```

---
