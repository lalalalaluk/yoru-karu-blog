# Markdown 語法練習


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

&lt;!--more--&gt;

&lt;!--
這是一個註釋
--&gt;

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

在要引用的文字前添加 `&gt;`。

&gt; **Fusion Drive** 結合了一個硬碟和一個快閃存儲（固態硬碟），並將其顯示為一個邏輯卷，兩個硬碟的空間結合在一起。

```
&gt; **Fusion Drive** 結合了一個硬碟和一個快閃存儲（固態硬碟），並將其顯示為一個邏輯卷，兩個硬碟的空間結合在一起。
```

區塊引用也可以嵌套：

&gt; Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue. Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
&gt;
&gt; &gt; Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.
&gt;
&gt; Mauris sit amet ligula egestas, feugiat metus tincidunt, luctus libero. Donec congue finibus tempor. Vestibulum aliquet sollicitudin erat, ut aliquet purus posuere luctus。

```
&gt; Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue. Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
&gt;
&gt; &gt; Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.
&gt;
&gt; Mauris sit amet ligula egestas, feugiat metus tincidunt, luctus libero. Donec congue finibus tempor. Vestibulum aliquet sollicitudin erat, ut aliquet purus posuere luctus。

```

# 清單

## 無序清單

一組無需順序的項目。

你可以使用以下任意符號來表示每個清單項目：

* 有效的項目符號
- 有效的項目符號
&#43; 有效的項目符號

```
* 有效的項目符號
- 有效的項目符號
&#43; 有效的項目符號
```

例如：

&#43; Lorem ipsum dolor sit amet
&#43; Consectetur adipiscing elit
&#43; Integer molestie lorem at massa
&#43; Facilisis in pretium nisl aliquet
&#43; Nulla volutpat aliquam velit
  - Phasellus iaculis neque
  - Purus sodales ultricies
  - Vestibulum laoreet porttitor sem
  - Ac tristique libero volutpat at
&#43; Faucibus porta lacus fringilla vel
&#43; Aenean sit amet erat nunc
&#43; Eget porttitor lorem

```
&#43; Lorem ipsum dolor sit amet
&#43; Consectetur adipiscing elit
&#43; Integer molestie lorem at massa
&#43; Facilisis in pretium nisl aliquet
&#43; Nulla volutpat aliquam velit
  - Phasellus iaculis neque
  - Purus sodales ultricies
  - Vestibulum laoreet porttitor sem
  - Ac tristique libero volutpat at
&#43; Faucibus porta lacus fringilla vel
&#43; Aenean sit amet erat nunc
&#43; Eget porttitor lorem
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
      assets: &#39;docs/assets&#39;,
      data: &#39;src/data/*.{json,yml}&#39;,
      helpers: &#39;src/custom-helpers.js&#39;,
      partials: [&#39;src/partials/**/*.{hbs,md}&#39;]
    },
    pages: {
      options: {
        layout: &#39;default.hbs&#39;
      },
      files: {
        &#39;./&#39;: [&#39;src/templates/pages/index.hbs&#39;]
      }
    }
  }
};
```




---

> Author: luk  
> URL: http://localhost:1313/posts/markdown-practice/  

