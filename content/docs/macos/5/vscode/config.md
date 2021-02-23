---
weight: 10
title: "配置"
bookCollapseSection: true
---

# VSCode 配置

`settings.json`

```json
{
  "gitlens.advanced.messages": {
    "suppressShowKeyBindingsNotice": true
  },
  "gitlens.historyExplorer.enabled": true,
  "java.errors.incompleteClasspath.severity": "ignore",
  "materialTheme.autoApplyIcons": true,
  "workbench.colorCustomizations": {},
  "materialTheme.accentPrevious": "Breaking Bad",
  "workbench.colorTheme": "Material Theme",
  "materialTheme.fixIconsRunning": false,
  // Controls the font family.
  "editor.fontFamily": "Consolas",
  "editor.lineHeight": 22,
  "window.zoomLevel": 0,
  "editor.fontSize": 14,
  "workbench.startupEditor": "newUntitledFile",
  "editor.suggestSelection": "first",
  "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue",
  "python.jediEnabled": false,
  "leetcode.endpoint": "leetcode-cn",
  "python.linting.pylintEnabled": true,
  "leetcode.defaultLanguage": "golang",
  "leetcode.hint.configWebviewMarkdown": false,
  "leetcode.hint.commentDescription": false,
  "go.useLanguageServer": true,
  "[go]": {
    "editor.formatOnSave": true,
    "editor.codeActionsOnSave": {
      "source.organizeImports": true
    },
    // Optional: Disable snippets, as they conflict with completion ranking.
    "editor.snippetSuggestions": "none"
  },
  "[go.mod]": {
    "editor.formatOnSave": true,
    "editor.codeActionsOnSave": {
      "source.organizeImports": true
    }
  },
  "gopls": {
    // Add parameter placeholders when completing a function.
    "usePlaceholders": true,

    // If true, enable additional analyses with staticcheck.
    // Warning: This will significantly increase memory usage.
    "staticcheck": false
  },
  "leetcode.workspaceFolder": "/Users/yewang/.leetcode",
  "leetcode.hint.commandShortcut": false,
  // Configure glob patterns for excluding files and folders.
  // For example, the files explorer decides which files and folders to show or hide based on this setting.
  // Read more about glob patterns [here](https://code.visualstudio.com/docs/editor/codebasics#_advanced-search-options).
  "files.exclude": {
    "**/.git": true,
    "**/.svn": true,
    "**/.hg": true,
    "**/CVS": true,
    "**/.DS_Store": true,
    "**/.classpath": true,
    "**/.project": true,
    "**/.settings": true,
    "**/.factorypath": true
  },
  "http.proxy": "http://127.0.0.1:8081",
  "terminal.integrated.inheritEnv": true,
  "terminal.integrated.shell.osx": "/bin/zsh",
  // 为了使用 agnoster zsh 主题
  "terminal.integrated.fontFamily": "Meslo LG M DZ for Powerline",
  "terminal.integrated.rendererType": "dom",
  // 选中即复制
  "terminal.integrated.copyOnSelection": true,
  "sourcetrail.startServerAtStartup": true,
  // vim
  "vim.normalModeKeyBindingsNonRecursive": [
    {
      "before": [":"],
      "commands": ["workbench.action.showCommands"]
    },
    {
      "before": ["<leader>", "m"],
      "commands": ["bookmarks.toggle"]
    },
    {
      "before": ["<leader>", "b"],
      "commands": ["bookmarks.list"]
    },
    {
      "before": ["Z", "Z"],
      "commands": [":wq"]
    },
    {
      "before": ["<C-n>"],
      "commands": [":nohl"]
    },
    {
      "before": ["leader", "w"],
      "commands": ["workbench.action.files.save"]
    }
  ],
  // 无法兼容 R 插入模式
  // "vim.insertModeKeyBindings": [
  //     {
  //         "before": ["j", "j"],
  //         "after": ["<Esc>"]
  //     }
  // ],
  "vim.visualModeKeyBindingsNonRecursive": [
    {
      "before": ["p"],
      "after": ["p", "g", "v", "y"]
    },
    {
      "before": [">"],
      "commands": ["editor.action.indentLines"]
    },
    {
      "before": ["<"],
      "commands": ["editor.action.outdentLines"]
    }
  ],
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,
  "markdown-preview-enhanced.automaticallyShowPreviewOfMarkdownBeingEdited": false,
  "markdown.extension.preview.autoShowPreviewToSide": false,
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  // Activate Python Environment in Terminal created using the Extension.
  "python.terminal.activateEnvironment": false,
  // Path to folder with a list of Virtual Environments (e.g. ~/.pyenv, ~/Envs, ~/.virtualenvs).
  "python.venvPath": "~/.local/share/virtualenvs",
  "editor.largeFileOptimizations": false,
  "C_Cpp.updateChannel": "Insiders",
  "[markdown]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  // Format a file on save. A formatter must be available, the file must not be saved after delay, and the editor must not be shutting down.
  "editor.formatOnSave": false,
  "[cpp]": {
    "editor.defaultFormatter": "ms-vscode.cpptools"
  },
  "clang-format.executable": "/Users/yewang/.vscode/extensions/ms-vscode.cpptools-0.27.0-insiders3/LLVM/bin/clang-format.darwin",
  "[json]": {
    "editor.defaultFormatter": "HookyQR.beautify"
  },
  // markdownlint config object
  "markdownlint.config": {
    "MD004": false,
    "MD013": false,
    "MD024": false,
    "MD025": false,
    "MD026": false,
    "MD040": false,
    "MD045": false
  },
  "markdownlint.run": "onSave",
  "window.title": "${dirty} ${activeEditorMedium}${separator}${rootName}",
  // 右侧概览 用色块代替缩小的字符; 设置水平最大列数; 始终显示滑块
  "editor.minimap.renderCharacters": false,
  "editor.minimap.maxColumn": 200,
  "editor.minimap.showSlider": "always",
  // 标签
  "editor.smoothScrolling": true,
  "editor.cursorBlinking": "phase",
  // "editor.cursorSmoothCaretAnimation": true,
  // 最后一行
  "files.insertFinalNewline": true,
  // 取消最后空格
  "files.trimTrailingWhitespace": true,
  // 取消发送给 ms
  "telemetry.enableCrashReporter": false,
  "telemetry.enableTelemetry": false,
  "workbench.settings.enableNaturalLanguageSearch": false,
  // "editor.renderWhitespace": "all",

  // Fit code within this line limit
  // "prettier.printWidth": 80,
  // Controls the wrapping column of the editor when `editor.wordWrap` is `wordWrapColumn` or `bounded`.
  // "editor.wordWrapColumn": 80,

  "python.formatting.autopep8Args": ["--max-line-length=100"],
  "javascript.updateImportsOnFileMove.enabled": "always",
  "[javascript]": {
    "editor.defaultFormatter": "HookyQR.beautify"
  },
  "java.requirements.JDK11Warning": false,
  "[java]": {
    "editor.defaultFormatter": "redhat.java"
  },
  "[yaml]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "java.semanticHighlighting.enabled": true,
  "extensions.ignoreRecommendations": true,
  "python.languageServer": "Pylance",
  "java.project.importOnFirstTimeStartup": "automatic",
  "picgo.picBed.current": "github",
  "picgo.picBed.github.repo": "ikingye/imagehost",
  "picgo.picBed.github.token": "xxx",
  "picgo.picBed.github.branch": "master",
  "picgo.picBed.github.customUrl": "https://cdn.jsdelivr.net/gh/ikingye/imagehost",
  "picgo.picBed.github.path": "picgo/",
  "picgo.customOutputFormat": "![](${url})",
  "csharp.suppressDotnetInstallWarning": true,
  "csharp.suppressDotnetRestoreNotification": true,
  "go.goroot": "/usr/local/Cellar/go/1.14.6/libexec",
  "sonarlint.rules": {
    "Web:LinkToImageCheck": {
      "level": "off"
    }
  },
  "python.showStartPage": false,
  "hediet.vscode-drawio.local-storage": "xxx",
  "hediet.vscode-drawio.codeLinkActivated": true,
  // Configure which editor to use for specific file types.
  "workbench.editorAssociations": [
    {
      "viewType": "hediet.vscode-drawio-text",
      "filenamePattern": "*.svg"
    },
    {
      "viewType": "hediet.vscode-drawio-text",
      "filenamePattern": "*.drawio"
    }
  ],
  "todo-tree.tree.showScanModeButton": false,
  "[dockerfile]": {
    "editor.defaultFormatter": "ms-azuretools.vscode-docker"
  },
  "jupyter.sendSelectionToInteractiveWindow": true,
  "pasteImage.defaultName": "YMMDDHHmmss",
  "pasteImage.path": "${projectRoot}/static/image/2020",
  "jupyter.alwaysTrustNotebooks": true
}
```
