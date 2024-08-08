---
title: Markdown 語法練習
subtitle: 基本語法示例
date: 2024-08-09T02:21:00+08:00
slug: markdown-practice
draft: false

description: 本文介紹了 Markdown 的基本語法，包括標題、粗體、斜體、刪除線、區塊引用、清單、語法高亮、表格和鏈接。
keywords: markdown, 語法, 教程, 基本語法
tags:
    - markdown
    - 語法
    - 教程
categories:
    - 教程
    - markdown

# See details front matter: https://fixit.lruihao.cn/documentation/content-management/introduction/#front-matter
---

# 標題

標題從 h1 到 h6 通過 # 來表示每個級別：

# h1 標題
## h2 標題
### h3 標題
#### h4 標題
##### h5 標題
###### h6 標題

```
# h1 標題
## h2 標題
### h3 標題
#### h4 標題
##### h5 標題
###### h6 標題

```

<!--more-->

<!--
這是一個註釋
-->

# 分隔線
___ 
---
***

三種都可以

```
___ 
---
***
```

# 粗體

用粗體字來強調文字片段。

以下文字將被渲染為粗體文字。

**渲染為粗體文字**

```
**渲染為粗體文字**
```

# 斜體

用斜體字來強調文字片段。

以下文字將被渲染為斜體文字。

_渲染為斜體文字_
```
_渲染為斜體文字_
```

# 刪除線

在 GFM (GitHub 風格的 Markdown) 中可以使用刪除線。

~~刪除這段文字~~
```
~~刪除這段文字~~
```

# 區塊引用

用於在文檔中引用來自其他來源的內容。

在要引用的文字前添加 `>`。

> **Fusion Drive** 結合了一個硬碟和一個快閃存儲（固態硬碟），並將其顯示為一個邏輯卷，兩個硬碟的空間結合在一起。

```
> **Fusion Drive** 結合了一個硬碟和一個快閃存儲（固態硬碟），並將其顯示為一個邏輯卷，兩個硬碟的空間結合在一起。
```

區塊引用也可以嵌套：

> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue. Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
>
> > Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.
>
> Mauris sit amet ligula egestas, feugiat metus tincidunt, luctus libero. Donec congue finibus tempor. Vestibulum aliquet sollicitudin erat, ut aliquet purus posuere luctus。

```
> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue. Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
>
> > Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.
>
> Mauris sit amet ligula egestas, feugiat metus tincidunt, luctus libero. Donec congue finibus tempor. Vestibulum aliquet sollicitudin erat, ut aliquet purus posuere luctus。

```

# 清單

## 無序清單

一組無需順序的項目。

你可以使用以下任意符號來表示每個清單項目：

* 有效的項目符號
- 有效的項目符號
+ 有效的項目符號

```
* 有效的項目符號
- 有效的項目符號
+ 有效的項目符號
```

例如：

+ Lorem ipsum dolor sit amet
+ Consectetur adipiscing elit
+ Integer molestie lorem at massa
+ Facilisis in pretium nisl aliquet
+ Nulla volutpat aliquam velit
  - Phasellus iaculis neque
  - Purus sodales ultricies
  - Vestibulum laoreet porttitor sem
  - Ac tristique libero volutpat at
+ Faucibus porta lacus fringilla vel
+ Aenean sit amet erat nunc
+ Eget porttitor lorem

```
+ Lorem ipsum dolor sit amet
+ Consectetur adipiscing elit
+ Integer molestie lorem at massa
+ Facilisis in pretium nisl aliquet
+ Nulla volutpat aliquam velit
  - Phasellus iaculis neque
  - Purus sodales ultricies
  - Vestibulum laoreet porttitor sem
  - Ac tristique libero volutpat at
+ Faucibus porta lacus fringilla vel
+ Aenean sit amet erat nunc
+ Eget porttitor lorem
```

## 有序清單

一組有順序的項目。

1. Lorem ipsum dolor sit amet
4. Consectetur adipiscing elit
2. Integer molestie lorem at massa
8. Facilisis in pretium nisl aliquet
4. Nulla volutpat aliquam velit
99. Faucibus porta lacus fringilla vel
21. Aenean sit amet erat nunc
6. Eget porttitor lorem

```
1. Lorem ipsum dolor sit amet
4. Consectetur adipiscing elit
2. Integer molestie lorem at massa
8. Facilisis in pretium nisl aliquet
4. Nulla volutpat aliquam velit
99. Faucibus porta lacus fringilla vel
21. Aenean sit amet erat nunc
6. Eget porttitor lorem
```

# 程式語法

GFM (GitHub 風格的 Markdown) 支持語法高亮。要啟用它，只需在第一個代碼「圍欄」之後添加語言的文件擴展名，例如 ` ```js `，語法高亮將自動應用於渲染的 HTML 中。

例如，要對 JavaScript 代碼進行語法高亮：

```js
grunt.initConfig({
  assemble: {
    options: {
      assets: 'docs/assets',
      data: 'src/data/*.{json,yml}',
      helpers: 'src/custom-helpers.js',
      partials: ['src/partials/**/*.{hbs,md}']
    },
    pages: {
      options: {
        layout: 'default.hbs'
      },
      files: {
        './': ['src/templates/pages/index.hbs']
      }
    }
  }
};
```


