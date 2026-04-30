---
title: 'Markdown 样式指南'
description: '以下是在 Astro 中编写 Markdown 内容时可以使用的一些基本 Markdown 语法示例。'
pubDate: 'Jun 19 2024'
heroImage: '../../assets/blog-placeholder-1.jpg'
---

以下是在 Astro 中编写 Markdown 内容时可以使用的一些基本 Markdown 语法示例。

## 标题

以下 HTML `<h1>`—`<h6>` 元素代表六个级别的章节标题。`<h1>` 是最高级别，`<h6>` 是最低级别。

# 一级标题

## 二级标题

### 三级标题

#### 四级标题

##### 五级标题

###### 六级标题

## 段落

这是一段示例文字。Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

## 图片

### 语法

```markdown
![替代文本](./图片的完整或相对路径)
```

### 输出效果

![博客占位图](../../assets/blog-placeholder-about.jpg)

## 引用块

引用块元素表示从其他来源引用的内容，可以选择性地包含引用出处（必须在 `footer` 或 `cite` 元素内），也可以包含行内修改，如注释和缩写。

### 不带出处的引用

#### 语法

```markdown
> Tiam, ad mint andaepu dandae nostion secatur sequo quae.  
> **注意**你可以在引用块中使用 _Markdown 语法_。
```

#### 输出效果

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.  
> **注意**你可以在引用块中使用 _Markdown 语法_。

### 带出处的引用

#### 语法

```markdown
> 不要通过共享内存来通信，而要通过通信来共享内存。<br>
> — <cite>Rob Pike[^1]</cite>
```

#### 输出效果

> 不要通过共享内存来通信，而要通过通信来共享内存。<br>
> — <cite>Rob Pike[^1]</cite>

[^1]: 以上引言摘自 Rob Pike 在 2015 年 11 月 18 日 Gopherfest 上的[演讲](https://www.youtube.com/watch?v=PAAkCSZUG1c)。

## 表格

### 语法

```markdown
| 斜体      | 粗体     | 代码   |
| --------- | -------- | ------ |
| _斜体_    | **粗体** | `代码` |
```

### 输出效果

| 斜体      | 粗体     | 代码   |
| --------- | -------- | ------ |
| _斜体_    | **粗体** | `代码` |

## 代码块

### 语法

我们可以在新行中使用 3 个反引号 ``` 开始代码片段，然后在新行中用 3 个反引号关闭。要高亮特定语言的语法，可以在前 3 个反引号后写上语言名称，例如 html、javascript、css、markdown、typescript、txt、bash。

````markdown
```html
<!doctype html>
<html lang="zh-CN">
  <head>
    <meta charset="utf-8" />
    <title>HTML5 文档示例</title>
  </head>
  <body>
    <p>测试</p>
  </body>
</html>
```
````

### 输出效果

```html
<!doctype html>
<html lang="zh-CN">
  <head>
    <meta charset="utf-8" />
    <title>HTML5 文档示例</title>
  </head>
  <body>
    <p>测试</p>
  </body>
</html>
```

## 列表类型

### 有序列表

#### 语法

```markdown
1. 第一项
2. 第二项
3. 第三项
```

#### 输出效果

1. 第一项
2. 第二项
3. 第三项

### 无序列表

#### 语法

```markdown
- 列表项
- 另一项
- 再一项
```

#### 输出效果

- 列表项
- 另一项
- 再一项

### 嵌套列表

#### 语法

```markdown
- 水果
  - 苹果
  - 橙子
  - 香蕉
- 乳制品
  - 牛奶
  - 奶酪
```

#### 输出效果

- 水果
  - 苹果
  - 橙子
  - 香蕉
- 乳制品
  - 牛奶
  - 奶酪

## 其他元素 — abbr、sub、sup、kbd、mark

### 语法

```markdown
<abbr title="图形交换格式">GIF</abbr> 是一种位图图像格式。

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

按下 <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>Delete</kbd> 结束会话。

大多数<mark>蝾螈</mark>是夜行性的，以昆虫、蠕虫和其他小型生物为食。
```

### 输出效果

<abbr title="图形交换格式">GIF</abbr> 是一种位图图像格式。

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

按下 <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>Delete</kbd> 结束会话。

大多数<mark>蝾螈</mark>是夜行性的，以昆虫、蠕虫和其他小型生物为食。
