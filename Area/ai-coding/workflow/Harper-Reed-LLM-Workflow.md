---
tags: [ai-coding, workflow, prompt-engineering]
source: https://harper.blog/2025/02/16/my-llm-codegen-workflow-atm/
issue: "#14"
---

# Harper Reed 的 LLM 代码生成工作流

三步离散循环，TDD 优先。

## 工作流

### Step 1: Idea Honing（打磨想法）
用对话式 LLM（ChatGPT）逐问逐答打磨创意，"一次只问一个问题"，最后编译成 `spec.md`。

### Step 2: Planning（规划）
将 spec 交给推理模型（o1/o3/r1）拆解为小步骤的 prompt 序列（`prompt_plan.md`）+ `todo.md` 清单。每步足够小以确保安全测试，又足够大以推进项目。

### Step 3: Execution（执行）
逐个 prompt 喂给代码生成 LLM（Aider/Claude），每步构建在前一步之上。

## 遗留代码场景
先让 AI 分析现有代码库生成文档，再规划改动。可用 repomix 打包代码上下文。

## 关联
- [[Ralph-Wiggum-AI-Loop]] — 更激进的自动化迭代方式
- [[Shipping-With-Claude]] — 生产环境的三种姿态
