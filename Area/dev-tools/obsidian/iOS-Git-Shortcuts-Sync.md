---
tags: [obsidian, ios, git, sync]
source: https://utgd.net/article/20315
issue: "#7"
---

# Obsidian iOS + Git + Shortcuts 自动同步

通过 iOS Shortcuts 实现 Obsidian 打开时自动 git pull、关闭时自动 commit + push。

## 方案
- 创建两个 Shortcuts：「拉取 Obsidian」和「推送 Obsidian」
- 利用 iOS 自动化触发：打开 Obsidian 时 pull，关闭时 commit + push
- 需要 Working Copy 等支持 git 的 app
