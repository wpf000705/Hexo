---
title: 使用 Hexo Theme Fluid 开启技术博客
date: 2026-05-29 10:00:00
updated: 2026-05-29 10:00:00
categories:
  - 技术笔记
tags:
  - Hexo
  - Fluid
  - 博客搭建
---

这是 BLOG_TITLE 的第一篇示例文章。它用来确认 Hexo、Fluid 主题、分类、标签、归档和文章页目录都能正常工作。

<!-- more -->

## 为什么写博客

技术博客适合沉淀这些内容：

- 项目复盘：记录背景、方案、取舍和结果。
- 学习笔记：把零散知识整理成可复用的路径。
- 问题排查：保存报错、定位过程和最终修复方式。
- 工具清单：持续更新自己真正用过的开发工具。

## 推荐文章结构

一篇技术文章可以从四个部分开始：

1. 问题是什么。
2. 当前环境和约束是什么。
3. 解决方案如何落地。
4. 后续还能怎样优化。

## 示例代码块

```bash
npm run clean
npm run build
npm run server
```

Fluid 会为代码块提供高亮、行号和复制按钮。发布新文章时，可以通过下面的命令创建草稿：

```bash
npx hexo new "文章标题"
```

## 下一步

把 `BLOG_TITLE`、`AUTHOR_NAME`、`BLOG_SUBTITLE`、`BLOG_DESCRIPTION`、`GITHUB_URL`、`EMAIL_ADDRESS` 等占位符替换成真实信息，然后推送到 Git 仓库并连接 Vercel。
