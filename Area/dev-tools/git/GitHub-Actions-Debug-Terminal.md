---
tags: [github-actions, ci-cd, webrtc, debugging]
source: https://blog.gripdev.xyz/2026/01/10/actions-terminal-on-failure-for-debugging/
issue: "#36"
---

# GitHub Actions 失败时的调试终端

开源工具，当 GitHub Actions 构建失败时，通过 WebRTC P2P 连接获得交互式 Web 终端。

## 核心痛点
CI 失败后只能 push 猜测性修改 → 等结果 → 再猜，效率极低。

## 技术方案
- WebRTC UDP 打洞建立 P2P 连接，无需中继服务器
- 浏览器端 GitHub OAuth 验证，Actions 端 OIDC token 验证
- 只需在 workflow 中添加 `permissions: id-token: write`

## 链接
https://actions-term.gripdev.xyz/
