---
tags: [shell, fzf, productivity]
source: https://tratt.net/laurie/blog/2025/better_shell_history_search.html
issue: "#10"
---

# fzf + Ctrl-R 改善 Shell 历史搜索

作者称效率一夜翻倍，且长期效果更大——因为知道能找回命令，所以敢用更复杂的命令行。

## 默认 Ctrl-R 的问题
只能子串匹配，无法跨词搜索（如知道命令是 `cat`、文件名含 `motd` 但忘了目录）。

## fzf 的两个改变
1. 模糊匹配（输入"c mo"匹配 `cat /etc/motd`）
2. 同时显示多个结果

## 长期行为改变
不再设全局环境变量，敢用更复杂的命令组合。

## 进阶
- skim（fzf 的 Rust 替代品）
- Atuin（跨机器同步历史记录）

## 关联
- [[Bash-Zsh-Tab-Completion]] — shell 效率的另一个维度
