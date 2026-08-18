---
title: Mizuki 使用简易指南
published: 2026-08-16
description: "本博客模板的使用教程。"
image: "./cover.webp"
tags: ["Mizuki", "博客写作", "自定义"]
category: 教程
draft: false
---

本博客模板基于 [Astro](https://astro.build/) 构建。如果本指南没有覆盖到你的问题，可以查阅 [Astro 官方文档](https://docs.astro.build/) 获取更多信息。

## 文章的 Front‑Matter（头部元信息）
```yaml
---
title: 我的第一篇博客文章
published: 2026-08-16
description: 这是我新Astro博客的第一篇文章。
image: ./cover.jpg
tags: [标签一, 标签二]
category: 前端
draft: false
---
```

| 参数          | 说明                                                         |
| ------------- | ------------------------------------------------------------ |
| `title`       | 文章标题                                                     |
| `published`   | 文章发布日期                                                 |
| `pinned`      | 是否将文章置顶到文章列表顶部                                 |
| `priority`    | 置顶文章优先级，数值越小优先级越高（0、1、2……）              |
| `description` | 文章简短描述，将展示在首页列表                               |
| `image`       | 文章封面图片路径<br />1. 以`http://`/`https://`开头：使用网络图片<br />2. 以`/`开头：读取`public`目录内图片<br />3. 不带上述前缀：路径相对于当前md文件 |
| `tags`        | 文章标签                                                     |
| `category`    | 文章分类                                                     |
| `licenseName` | 文章内容的版权协议名称                                       |
| `author`      | 文章作者                                                     |
| `sourceLink`  | 文章引用来源链接                                             |
| `draft`       | 是否为草稿；草稿文章不会对外显示                             |

## 文章文件存放位置
你的文章文件需要放置在 `src/content/posts/` 目录下。你也可以新建子文件夹，方便整理文章与图片资源。
```
src/content/posts/
├── post‑1.md
└── post‑2/
    ├── cover.webp
    └── index.md
```
```

欢迎来到我的小站。
```
