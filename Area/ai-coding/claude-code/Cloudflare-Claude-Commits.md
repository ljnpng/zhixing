---
tags: [ai-coding, git, prompt-as-code]
source: https://www.maxemitchell.com/writings/i-read-all-of-cloudflares-claude-generated-commits/
issue: "#3"
---

# Cloudflare 的 Claude 生成 Commits 分析

作者逐条阅读了 Cloudflare 开源 OAuth 2.1 库约 50 个由 Claude 生成的 commit。

## 关键发现
- **每次 commit 都包含生成代码的 prompt**——git 历史从"变更记录"变成"意图记录"
- 以示例代码作为 prompt 效果最佳（"展示编舞而非描述舞蹈"）
- 最有效的反馈模式：「你做了 X，但应该做 Y，请修复」
- 文档生成几乎零成本

## AI 的短板
- 移动类声明等结构性操作需人工介入
- 约 40 个 commit 后手动修复变得频繁
- 样式和清理工作仍需人类

## 前瞻
如果把 prompt 当作源代码版本控制，模型升级后可以重新生成整个代码库。

## 关联
- [[Claude-As-Computer]] — 另一个重度使用者的经验
- [[Harper-Reed-LLM-Workflow]] — 也强调 prompt 的结构化管理
