---
tags: [shell, bash, zsh, cli]
source: https://mill-build.org/blog/14-bash-zsh-completion.html
issue: "#22"
---

# Bash/Zsh Tab 补全编写指南

为 CLI 工具编写跨 Bash/Zsh 的 Tab 补全，包括补全描述显示。

## 痛点
Bash 和 Zsh 的补全 API 完全不同，且 Bash 默认不支持补全描述。

## 解决方案
当只有一个匹配结果时，添加"虚拟"补全项触发 shell 显示描述文本。

## 实现
- Bash：`complete -F`
- Zsh：`compadd -d`

## 关联
- [[fzf-History-Search]] — shell 效率的另一个维度
