---
title: 测试博客 - 第0篇
date: 2026-09-14 02:17:39
tags: [测试]
categories: [技术]
---

# 这是一个博客文章的测试
此处测试实际内容

## 这同样是我的第0篇博客
以后博客标题命名以【name - 第x篇】的方式命名

## 如何创建新的博客文章
流程（此处为PC端）：
1. 生成新文章
   ./node_modules/.bin/hexo new post "Ciallo～(∠・ω<)⌒★"
2. 编辑 front-matter
   ```
   它改成类似这样（标题中文、补上标签和分类）：
  	---
  	title: 我的第一篇博客
  	date: 2026-09-14 00:00:00
  	tags: [随笔]（随便写，标签而已）
  	categories: [随笔]（某几个大类的分类，目前有【技术】【随笔】。。。后续可再加，但别太多）
   ---
   ```
3. 写正文（Markdown，就写在 front-matter 下面）
4. 本地预览（发布前先看一眼） 
   ```
   ./node_modules/.bin/hexo generate
   ./node_modules/.bin/hexo server
   ```
   浏览器打开 http://localhost:4000，Ctrl+F5
   硬刷新，确认新文章出现在首页、点进去排版正常。看完按 Ctrl+C 停掉 server。
5. 发布上线
   git add .
   git commit -m 'Ciallo～(∠・ω<)⌒★'
   git push

## 还有一些小细节，一起讲
1. date 是实时的
2. tags 可以随便打，标签来的
3. categories 不能乱来，这是大分类，只保留几个就够，目前仅有【随笔】【技术】，后续视情况再添加
4. markdown 简单小用法一览
e.g.
- 测试列表1
- 测试列表2
- 测试列表3

**文字加粗**
*文字斜体*

> 引用测试

行内代码 `npm install` 和代码块：

```bash
echo "Hello, Hexo!"
```