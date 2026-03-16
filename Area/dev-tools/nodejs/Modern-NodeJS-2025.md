---
tags: [nodejs, javascript, best-practices]
source: https://kashw1n.com/blog/nodejs-2025/
issue: "#20"
---

# Modern Node.js Patterns 2025

核心趋势：减少外部依赖，全面拥抱 Web 标准。

## 关键变化
- **ESM + `node:` 前缀**替代 CommonJS：`import { readFile } from "node:fs/promises"`
- **内置 Fetch API** 替代 axios/node-fetch：`AbortSignal.timeout(5000)` 内置超时
- **Top-Level Await**：不再需要 IIFE 包装异步初始化
- **AbortController**：标准化的操作取消机制

## 方向
Node.js 正在和浏览器 API 对齐，跨环境一致性越来越好。
