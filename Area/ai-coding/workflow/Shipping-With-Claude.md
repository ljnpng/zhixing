---
tags: [ai-coding, claude, testing, best-practices]
source: https://diwank.space/field-notes-from-shipping-real-code-with-claude
issue: "#15"
---

# 用 Claude 交付生产代码的实战笔记

Julep 团队的实战经验。核心洞察：好的工程实践是 AI 放大能力而非放大混乱的前提。

## 三种姿态
1. **First-Drafter**：写样板代码、脚本，放飞自我
2. **Pair-Programmer**：<5000 行项目，依赖 CLAUDE.md 和锚点注释 `AIDEV-NOTE`
3. **Validator**：代码审查

## 铁律
- **自己写测试是神圣不可侵犯的**——唯一能确保 AI 产出质量的锚点
- 严格实践的团队部署频率提升 46 倍，commit 到部署快 440 倍

## 关联
- [[TDD-Agent-Protocol]] — TDD 行为准则，和"自己写测试"的理念一致
- [[Harper-Reed-LLM-Workflow]] — 另一种结构化工作流
- [[AGENTS-md-vs-Skills]] — CLAUDE.md 的上下文管理策略
