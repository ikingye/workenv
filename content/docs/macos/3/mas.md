---
weight: 20
title: "Mas"
bookCollapseSection: true
---

# [mas-cli/mas](https://github.com/mas-cli/mas) ![Github stars](https://img.shields.io/github/stars/mas-cli/mas.svg)

Each application in the Mac App Store has a product identifier which is also used for mas-cli commands.
Using mas list will show all installed applications and their product identifiers.

```shell
$ mas list
446107677 Screens
407963104 Pixelmator
497799835 Xcode

$ mas search Xcode
497799835 Xcode
688199928 Docs for Xcode
449589707 Dash 3 - API Docs & Snippets. Integrates with Xcode, Alfred, TextWrangler and many more.
[...]

$ mas install 808809998
==> Downloading PaintCode 2
==> Installed PaintCode 2

# If you want to install the first result that the search command returns, use the lucky command.
$ mas lucky twitter
==> Downloading Twitter
==> Installed Twitter

$ mas outdated
497799835 Xcode (7.0)
446107677 Screens VNC - Access Your Computer From Anywhere (3.6.7)

$ mas upgrade
Upgrading 2 outdated applications:
Xcode (7.0), Screens VNC - Access Your Computer From Anywhere (3.6.7)
==> Downloading Xcode
==> Installed Xcode
==> Downloading iFlicks
==> Installed iFlicks

$ mas upgrade 715768417
Upgrading 1 outdated application:
Xcode (8.0)
==> Downloading Xcode
==> Installed Xcode

$ mas signin mas@example.com
==> Signing in to Apple ID: mas@example.com
Password:
```
