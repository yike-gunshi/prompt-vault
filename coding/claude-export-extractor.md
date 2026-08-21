---
title: Claude 导出数据批量提取
summary: 从 Claude 官方导出的 JSON 数据包批量提取对话，过滤分类后转成可读 Markdown 并沉淀可复用知识
category: coding
tags: [Claude, 数据导出, Markdown, 记忆沉淀]
model: 
source_name: 飞书 · claude本地内容导出
source_url: https://my.feishu.cn/wiki/H3YfwgOfriTNmakFaQxcegcunvg
collected: 2026-08-20
media: 0
---

# Claude 导出数据批量提取

> 把 Claude 官方导出的 JSON 数据包批量转成可读 Markdown：解析嵌套结构、过滤空对话、按主题分类，最后把可复用知识存入持久化 memory。

## Prompt 原文

```text
从Claude导出的JSON数据包中批量提取对话：

解析conversations.json、zip包内嵌套的conversations/projects/design_chats，

按内容量过滤空对话，按主题分类（工具/创作/设计/闲聊），

导出为可读markdown，

最后筛选出可复用的知识（个人画像、技术决策、风格规范）存入持久化memory。
```

## 来源

- 出处：[飞书 · claude本地内容导出](https://my.feishu.cn/wiki/H3YfwgOfriTNmakFaQxcegcunvg)
- 收录：2026-08-20
