---
tags: [ai-coding, agents-md, context-management]
source: https://vercel.com/blog/agents-md-outperforms-skills-in-our-agent-evals
---

# AGENTS.md vs Skills — 被动上下文完胜主动检索

Vercel 针对 Next.js 16 API 的严谨 eval。

## 结果
| 方案 | 通过率 |
|------|--------|
| 基线（无文档） | 53% |
| Skills（默认） | 53%（56% 情况下根本不调用） |
| Skills + 显式指令 | 79%（但措辞脆弱） |
| **AGENTS.md 文档索引** | **100%** |

## 为什么被动上下文赢了
1. **没有决策点**——agent 不需要判断"要不要查文档"
2. **每轮对话都可用**——不像 skill 需要异步加载
3. **没有顺序问题**——skill 会引入"先查文档还是先看项目"的纠结

## 实用技巧
- 40KB 文档压缩到 8KB（管道分隔符格式），通过率不变
- 不是全部文档塞进去，而是放索引，agent 需要时再读具体文件
- 关键指令：`Prefer retrieval-led reasoning over pre-training-led reasoning`

## 关联
- [[AI-Zealotry-Rocklin]] — Hooks 是 CLAUDE.md 的补充方案
- [[Cursor-RIPER-Protocol]] — 另一种上下文管理策略
- [[Shipping-With-Claude]] — CLAUDE.md 的实战用法
