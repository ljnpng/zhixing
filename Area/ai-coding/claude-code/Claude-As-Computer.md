---
tags: [ai-coding, claude-code, automation, git]
source: https://steipete.me/posts/2025/claude-code-is-my-computer
issue: "#8"
---

# Claude Code Is My Computer

PSPDFKit 创始人 Peter Steinberger 用 `--dangerously-skip-permissions` 跑 Claude Code 两个月零事故。

## 用途远超编码
- 迁移 Mac 环境
- 批量转换 Jekyll 到 MDX 博客
- 提取 Swift 开源库
- 自动 git commit/PR/CI 修复
- 配置 macOS 系统设置

## 核心技巧
- **"commit everything in logical chunks"**——Claude 自动分组 staging、写 commit message、push、开 PR、监控 CI、修 CI 失败
- Wispr Flow 语音输入 + Claude Code 写博客
- CLAUDE.md 维护好项目上下文是关键
- agent-rules 仓库：github.com/steipete/agent-rules

## 风险管理
Arq 每小时快照 + SuperDuper 克隆。$200/月 Max 计划每天省一小时。

## 关联
- [[Cursor-vs-Claude-Code]] — 工具选择对比
- [[Ralph-Wiggum-AI-Loop]] — 类似的自动化思路
- [[Cloudflare-Claude-Commits]] — 也是重度 git 自动化
