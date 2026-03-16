---
tags: [ai-coding, claude-code, workflow]
source: https://matthewrocklin.com/ai-zealotry/
issue: "#33"
---

# AI Zealotry — 停止做简单的事

Dask 创始人 Matthew Rocklin 的 AI 开发实践。核心观点：资深工程师最应该用 AI——你有足够判断力避免 AI slop，又有大量可释放的生产力。

## 核心心法
- **停止做简单的事**——不断识别和拒绝简单任务，攀爬抽象阶梯
- 不看代码也能建立信心：通过测试、质询 AI、简化、技术债清理
- 放弃 Python 转向 Rust/TypeScript——AI 消除了 Python 的易用性优势，类型系统为 AI 提供更好的反馈

## Hooks > CLAUDE.md
- AI 经常忘记 CLAUDE.md 里的指令，用 Hooks 强制执行规则更可靠
- PreToolUse 钩子拦截错误命令
- Python 脚本覆盖权限系统（支持正则和任意逻辑）
- 声音钩子在 Claude 完成时通知开发者

## 关联
- [[Cursor-vs-Claude-Code]] — 类似的"攀登抽象层级"思路
- [[AGENTS-md-vs-Skills]] — Hooks 是 CLAUDE.md 的补充方案
- [[Process-Before-AI]] — 都强调先理清思路再用工具
