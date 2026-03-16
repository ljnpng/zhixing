---
tags: [java, mybatis, mysql, json, bug]
source: https://juejin.cn/post/7054947458261975053
issue: "#13"
---

# MyBatis JSON 字段布尔值陷阱

`setBoolean` 将 `true` → `1`，`false` → `0`，但 MySQL JSON 中 `1` 和 `true` 是不同的值。

## 问题
实际生成的 SQL：`WHERE task_params -> '$.online' = '1'` 而非 `= 'true'`，导致查询匹配失败。

## 解决方案
用字符串类型传参，或在 SQL 中用 `JSON_EXTRACT` + `CAST` 做类型转换。
