---
tags: [python, uv, scripting]
source: https://blog.dusktreader.dev/2025/03/29/self-contained-python-scripts-with-uv/
issue: "#9"
---

# uv + PEP 723 自包含 Python 脚本

在 shebang 行加入 uv，配合 `/// script` 元数据声明依赖，脚本可以直接运行并自动管理依赖。

## 用法

```python
#!/usr/bin/env -S uv run --script
# /// script
# requires-python = ">=3.8"
# dependencies = ["requests", "rich"]
# ///
```

配合 `chmod +x` 直接执行，无需手动管理 venv。

## 适用场景
一次性工具脚本、测试辅助脚本、运维脚本。
