---
tags: [ai-coding, claude-code, cursor]
source: https://blog.silennai.com/claude-code
issue: "#38"
---

# Cursor vs Claude Code

作者从 Cursor Top 0.01% 用户转向 Claude Code。核心原因：终端原生的异步优先思维强制你抽象到更高层次。

## Claude Code 优势
- **异步优先**：IDE 内操作容易陷入逐行审查的本能
- **模型针对自身脚手架做了 RLHF 优化**：Claude 在 Claude Code 里表现更好
- 成本效率更高、可定制性更强

## Cursor 仍有优势
- 像素级前端调整
- 学习场景
- 小改动避免上下文污染

## 推荐组合
Claude Code + Opus 做主力规划和复杂重构，Cursor + Sonnet 做紧反馈循环。

## 关联
- [[Claude-Code-Setup]] — Claude Code 基础配置
- [[Claude-As-Computer]] — Claude Code 的极限用法
- [[AI-Zealotry-Rocklin]] — 类似的"攀登抽象层级"思路
