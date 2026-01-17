---
title: "CSS 现代布局技术"
date: 2023-12-15T11:30:00+08:00
image_webp: images/blog/blog-post-5.webp
image: images/blog/blog-post-5.jpg
author: 张伟
description : "掌握 Flexbox、Grid 等现代 CSS 布局技术"
categories: ["Web开发", "设计"]
tags: ["CSS", "Flexbox", "Grid", "布局", "响应式"]
series: ["Web开发系列"]
---

CSS 布局技术在近年来有了巨大的进步。本文将介绍现代 CSS 布局的核心技术和应用场景。

## Flexbox 布局

Flexbox 适合一维布局：

```css
.flex-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 1rem;
}

.flex-item {
  flex: 1;
}
```

### 常见应用场景

- 导航栏
- 卡片布局
- 表单元素对齐

## Grid 布局

Grid 适合二维布局：

```css
.grid-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}
```

### Grid 的强大功能

- **命名网格线**：便于理解和维护
- **网格区域**：直观的布局定义
- **自动放置**：智能填充网格

## Container Queries

容器查询是响应式设计的未来：

```css
.card-container {
  container-type: inline-size;
}

@container (min-width: 600px) {
  .card {
    display: flex;
  }
}
```

## 总结

现代 CSS 布局技术为我们提供了强大而灵活的工具。掌握 Flexbox 和 Grid，可以轻松应对各种布局需求。
