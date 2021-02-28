---
weight: 1
title: "GitHub"
bookCollapseSection: true
---

# GitHub

## 设置代理

```shell
git config --global http.proxy "http://127.0.0.1:8081"
git config --global https.proxy "http://127.0.0.1:8081"

# socks5 代理（如 Shadowsocks）
git config --global http.proxy "socks5://127.0.0.1:1080"
git config --global https.proxy "socks5://127.0.0.1:1080"

# 取消代理
git config --global --unset http.proxy
git config --global --unset https.proxy
```

---

## 学习 Github

### [Github Learning Lab](https://lab.github.com/)

#### [Introduction to GitHub](https://lab.github.com/githubtraining/introduction-to-github)

---

## Github 工具

### [cli/cli](https://github.com/cli/cli) ![Github stars](https://img.shields.io/github/stars/cli/cli.svg)

GitHub’s official command line tool https://cli.github.com

### [github/hub](https://github.com/github/hub) ![Github stars](https://img.shields.io/github/stars/github/hub.svg)

A command-line tool that makes git easier to use with GitHub. https://hub.github.com/

---

## 开源库 素材 / 规范

### 徽章 [shields.io](https://shields.io/)

如：

![Github stars](https://img.shields.io/github/stars/doocs/advanced-java.svg)

参考：

- [用 [Substats] 和 Shields.io 为你的个人主页定制动态数据小牌子](https://sspai.com/post/59593)

  [spencerwooo/Substats](https://github.com/spencerwooo/Substats) ![Github stars](https://img.shields.io/github/stars/spencerwooo/Substats.svg)

---

### Github star 历史

#### [timqian/star-history](https://github.com/timqian/star-history) ![Github stars](https://img.shields.io/github/stars/timqian/star-history.svg)

https://star-history.t9t.io/

#### [vesoft-inc/github-statistics](https://github.com/vesoft-inc/github-statistics) ![Github stars](https://img.shields.io/github/stars/vesoft-inc/github-statistics.svg)

A react static app for displaying github repo statistiscs like Star History, Fork History and more.

https://vesoft-inc.github.io/github-statistics/

#### [antonmedv/spark](https://github.com/antonmedv/spark) ![Github stars](https://img.shields.io/github/stars/antonmedv/spark.svg)

[![GitHub Star Sparkline](https://stars.medv.io/servicemesher/istio-handbook.svg)](https://stars.medv.io/servicemesher/istio-handbook)

#### [seladb/startrack-js](https://github.com/seladb/startrack-js) ![Github stars](https://img.shields.io/github/stars/seladb/startrack-js.svg)

GitHub star history and stats - based on JavaScript only!

https://seladb.github.io/StarTrack-js/

#### [elliotreborn/github-stars](https://github.com/elliotreborn/github-stars) ![Github stars](https://img.shields.io/github/stars/elliotreborn/github-stars.svg)

技术栈的 star 趋势数据

---

### Github PR 统计

### 开源相关工作岗位

[t9tio/open-source-jobs](https://github.com/t9tio/open-source-jobs) ![Github stars](https://img.shields.io/github/stars/t9tio/open-source-jobs.svg)

A list of Open Source projects offering jobs. https://oo.t9t.io/organizations

---

### 角落标志 [tholman/github-corners](https://github.com/tholman/github-corners) ![Github stars](https://img.shields.io/github/stars/tholman/github-corners.svg)

[http://tholman.com/github-corners/](http://tholman.com/github-corners/)

如：
![](https://cdn.jsdelivr.net/gh/ikingye/imagehost/picgo/20200330145209.png)

---

## GitHub Apps

- Run persistently and can react to events quickly.
- Work great when persistent data is needed.
- Work best with API requests that aren't time consuming.
- Run on a server or compute infrastructure that you provide.

参考：

- [Strengths of GitHub Actions and GitHub Apps](https://help.github.com/en/actions/building-actions/about-actions#strengths-of-github-actions-and-github-apps)

### [Mergify](https://github.com/apps/Mergify)

Stop merging your pull requests manually.

We save your time by automatically merging, commenting, rebasing, updating, labeling, backporting, closing, assigning, your pull requests.

#### [Mergifyio/mergify-engine](https://github.com/Mergifyio/mergify-engine) ![Github stars](https://img.shields.io/github/stars/Mergifyio/mergify-engine.svg)

Engine for Mergify https://mergify.io

### [Netlify](https://github.com/apps/netlify)

### [wei/pull]

### [Pull](https://github.com/apps/pull)

Keep your forks up-to-date via automated PRs

[wei/pull](https://github.com/wei/pull) ![Github stars](https://img.shields.io/github/stars/wei/pull.svg)

### [probot/weekly-digest](https://github.com/probot/weekly-digest) ![Github stars](https://img.shields.io/github/stars/probot/weekly-digest.svg)

自动生成周报到 issue

## GitHub Actions

- Provide automation that can perform continuous integration and continuous deployment.
- Can run directly on runner machines or in Docker containers.
- Can include access to a clone of your repository, enabling deployment and publishing tools, code formatters, and command line tools to access your code.
- Don't require you to deploy code or serve an app.
- Have a simple interface to create and use secrets, which enables actions to interact with third-party services without needing to store the credentials of the person using the action.

---

## Github 工具开发

### webhook

#### [NetEaseGame/git-webhook](https://github.com/NetEaseGame/git-webhook) ![Github stars](https://img.shields.io/github/stars/NetEaseGame/git-webhook.svg)

使用 Python Flask + SQLAchemy + Celery + Redis + React 开发的用于迅速搭建并使用 WebHook 进行自动化部署和运维，支持 Github / GitLab / Gogs / GitOsc。 https://webhook.hust.cc/

若觉得 git-webhook 部署依然比较复杂，可以尝试更为简洁的 cli 版本 [hustcc/webhookit](https://github.com/hustcc/webhookit) ![Github stars](https://img.shields.io/github/stars/hustcc/webhookit.svg)

---

#### [github-webhook-handler](https://github.com/github-webhook-handler) ![Github stars](https://img.shields.io/github/stars/github-webhook-handler.svg)

Node.js web handler / middleware for processing GitHub Webhooks

---

#### [go-playground/webhooks](https://github.com/go-playground/webhooks) ![Github stars](https://img.shields.io/github/stars/go-playground/webhooks.svg)

Webhook receiver for GitHub, Bitbucket, GitLab, Gogs

---

#### [hustcc/webhookit](https://github.com/hustcc/webhookit) ![Github stars](https://img.shields.io/github/stars/hustcc/webhookit.svg)

Simple git webhook cli tool for automation tasks, bind git webhook to action.

---

### [gorda/issue-man](https://github.com/gorda/issue-man) ![Github stars](https://img.shields.io/github/stars/gorda/issue-man.svg)

---

### Building apps

参考：

- [Building apps](https://developer.github.com/apps/)

### Building actions

参考：

- [Building actions](https://help.github.com/en/actions/building-actions)
