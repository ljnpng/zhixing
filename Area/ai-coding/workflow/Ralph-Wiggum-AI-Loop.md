---
tags: [ai-coding, claude-code, automation]
source: https://awesomeclaude.ai/ralph-wiggum
issue: "#39"
---

# Ralph Wiggum — AI 循环迭代法

核心是一个 bash while 循环：`while :; do cat PROMPT.md | claude; done`

## 适用场景
有明确完成标准的任务（如让测试全部通过），可以挂着过夜跑。

## 关键要素
- **迭代 > 完美**：不追求一次完美，让循环去打磨
- **失败即数据**：确定性的失败是可预测且有信息量的
- **操作者技能决定成败**：prompt 要有清晰的完成标准和自我纠错模式
- 安全网：务必用 `--max-iterations` 防止无限循环

## 高级模式
- Git Worktree 并行开发
- 多阶段链式开发
- 隔夜批处理

## 实战
YC 黑客松一夜生成 6 个仓库，$297 API 费用交付 $50k 合同。

## 关联
- [[Harper-Reed-LLM-Workflow]] — 更结构化的三步法
- [[Claude-As-Computer]] — Steinberger 也用类似的自动化思路
