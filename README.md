# 人类的留给人类: Human-for-Humans

人类为人类而创造和服务，AI 为生产而使用。

Humans create and serve for humans. AI serves the production process.

## 项目定位

本项目用于记录各平台上经用户提交、审核后的疑似 AI 内容账号。

本项目的内容可用于制作用于屏蔽的非商业化的浏览器插件、工具等等。

当前采用简化结构：

```text
数据源/      # JSON，人工维护，保存完整账号信息
账号名单/    # Markdown，由 GitHub Actions 自动生成
规则/        # 收录、提交、申诉规则
```

## 提交方式

普通用户请通过 GitHub Issue 提交疑似账号。维护者审核后，将有效信息写入 `数据源/*.json`。

每个平台一个 JSON 文件，例如：

```text
数据源/抖音.json
数据源/哔哩哔哩.json
数据源/小红书.json
```

GitHub Actions 会根据 `提交人数` 自动生成三档名单：

```text
账号名单/一级疑似.md    # 1–5 人提交
账号名单/二级疑似.md    # 6–100 人提交
账号名单/三级疑似.md    # 101 人以上提交
```

## 排序规则

JSON 与 Markdown 均按 `排序名` 升序排列。中文账号建议在 `排序名` 中填写拼音，英文账号直接填写英文小写形式。

## License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0).

SPDX-License-Identifier: CC-BY-NC-4.0
