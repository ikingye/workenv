---
weight: 10
title: "MacOS"
bookCollapseSection: true
---

# MacOS

## Homebrew

[Homebrew/brew](https://github.com/Homebrew/brew) ![Github stars](https://img.shields.io/github/stars/Homebrew/brew.svg) ![Language](https://img.shields.io/github/languages/top/Homebrew/brew.svg) ![Last Tag](https://img.shields.io/github/v/tag/Homebrew/brew.svg?sort=semver) ![Last commit](https://img.shields.io/github/last-commit/Homebrew/brew.svg)

The missing package manager for macOS (or Linux)
https://brew.sh

---

## Oh My Zsh

https://ohmyz.sh/

```shell
https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh
```

```shell
# 提示符
export PROMPT='%{$fg[magenta]%}%(?..%?%1v)%n@%{$fg[green]%}%M:%{$fg[cyan]%}%c%{$reset_color%} $(git_prompt_info)'

# 设置默认 shell
sudo chsh -s /usr/bin/zsh
```

---

## iTerm2

https://www.iterm2.com/

---

## VSCode

[VSCode](https://github.com/Microsoft/vscode) ![Github stars](https://img.shields.io/github/stars/Microsoft/vscode.svg) + [`hugo`](https://github.com/gohugoio/hugo) ![Github stars](https://img.shields.io/github/stars/gohugoio/hugo.svg) ([`hugo-book`](https://github.com/alex-shpak/hugo-book) ![Github stars](https://img.shields.io/github/stars/alex-shpak/hugo-book.svg))

```shell
code --list-extensions
code --list-extensions --show-versions
```

参考：

- [Command line extension management](https://code.visualstudio.com/docs/editor/extension-gallery#_command-line-extension-management)

### VSCode 推荐插件

| 插件    | 类型                | 推荐 | 备注 |
| ------- | ------------------- | ---- | ---- |
| ESLint  | 格式化 - JavaScript | ★★★★ |      |
| TabNine | 代码补全            | ★★★★ |      |

#### ESLint

[Microsoft/vscode-eslint](https://github.com/Microsoft/vscode-eslint) ![Github stars](https://img.shields.io/github/stars/Microsoft/vscode-eslint.svg) ![Language](https://img.shields.io/github/languages/top/Microsoft/vscode-eslint.svg) ![Last Tag](https://img.shields.io/github/v/tag/Microsoft/vscode-eslint.svg?sort=semver) ![Last commit](https://img.shields.io/github/last-commit/Microsoft/vscode-eslint.svg)

#### TabNine

[codota/tabnine-vscode](https://github.com/codota/tabnine-vscode) ![Github stars](https://img.shields.io/github/stars/codota/tabnine-vscode.svg) ![Language](https://img.shields.io/github/languages/top/codota/tabnine-vscode.svg) ![Last Tag](https://img.shields.io/github/v/tag/codota/tabnine-vscode.svg?sort=semver) ![Last commit](https://img.shields.io/github/last-commit/codota/tabnine-vscode.svg)

Tabnine works with all major programming languages including JavaScript, Python, TypeScript, PHP, C/C++, HTML/CSS, Go, Java, Ruby, C#, Rust, SQL, Bash, Kotlin, Julia, Lua, OCaml, Perl, Haskell, and React.​

参考：

- [VSCode 插件列表](https://marketplace.visualstudio.com/search?target=VSCode&category=All%20categories&sortBy=Installs)

---
