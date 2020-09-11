---
layout: post
title: "Visual Studio Code Settings"
categories: vscode
---

1. Open Perferences `Ctrl + ,`
2. Search `terminal.integrated.windows`
3. Select `Edit in settings.json`
4. Update setting value to flavoured terminal like
```
"terminal.integrated.shell.windows": "C:\\WINDOWS\\System32\\cmd.exe",
// or bash
"terminal.integrated.shell.windows": "C:\\Program Files\\Git\\bin\\bash.exe",
```