---
title: [帮助文档]post.md写作指南
description: 如果你是第一次尝试写post，请参看本文。
author: PhotonYan
date: 2025-02-21 10:00:00 +0800
categories: [tutorial, post_writing] 
tags: [tutorial]
math: true
comments: true
---

上传至`github page`的`post`文件应当是一个名为`YYYY-MM-DD-Title.md`的`markdown`文件。其中，标题中的空格应当使用`-`或者`_`替代。

文件内容应当由两部分组成，分别是`yaml`标记与`markdown`正文。

以下是应当写在整个`.md`文件之前的标记。
```yaml
---
title: [课程测评]课程名称
description: 补充描述
author: 作者
date: 2025-02-21 10:00:00 +0800
categories: [course_feedback, collage] 
tags: [course_feedback]
math: true
comments: true
---
```

以下是可以用于编辑格式的`Markdown`记号：

## 各级标题

# H1 — 一级标题
{: .mt-4 .mb-0 }

## H2 — 二级标题
{: data-toc-skip='' .mt-4 .mb-0 }

### H3 — 三级标题
{: data-toc-skip='' .mt-4 .mb-0 }

#### H4 — 四级标题
{: data-toc-skip='' .mt-4 }
<!-- markdownlint-restore -->

## 正文

这里是正文。

## 列表环境

### 有序列表

1. Firstly
2. Secondly
3. Thirdly

### 无序列表

- Chapter
  - Section
    - Paragraph

### ToDo list

- [ ] Job
  - [x] Step 1
  - [x] Step 2
  - [ ] Step 3

### 定义

通班
: 北京大学通用人工智能实验班。

## 引用环境

> This line shows the _block quote_.

## 主题框

<!-- markdownlint-capture -->
<!-- markdownlint-disable -->
> An example showing the `tip` type prompt.
{: .prompt-tip }

> An example showing the `info` type prompt.
{: .prompt-info }

> An example showing the `warning` type prompt.
{: .prompt-warning }

> An example showing the `danger` type prompt.
{: .prompt-danger }
<!-- markdownlint-restore -->

## 列表

| Company                      | Contact          | Country |
| :--------------------------- | :--------------- | ------: |
| Alfreds Futterkiste          | Maria Anders     | Germany |
| Island Trading               | Helen Bennett    |      UK |
| Magazzini Alimentari Riuniti | Giovanni Rovelli |   Italy |

## 链接

<http://127.0.0.1:4000>

[名称](https://www.baidu.com)

## 注释

Click the hook will locate the footnote[^footnote], and here is another footnote[^fn-nth-2].

## 行内代码

This is an example of `Inline Code`.

## 代码框

### Common

```text
This is a common code snippet, without syntax highlight and line number.
```

### 选定代码框的语言

```bash
if [ $? -ne 0 ]; then
  echo "The command was not successful.";
  #do the needful / exit
fi;
```

### 更改标题

```sass
@import
  "colors/light-typography",
  "colors/dark-typography";
```
{: file='_sass/jekyll-theme-chirpy.scss'}

## 数学公式

本github page采用 [**MathJax**](https://www.mathjax.org/)构建 $\LaTeX$ 代码:

$$
\begin{equation}
  \sum_{n=1}^\infty 1/n^2 = \frac{\pi^2}{6}
  \label{eq:series}
\end{equation}
$$

We can reference the equation as \eqref{eq:series}.

When $a \ne 0$, there are two solutions to $ax^2 + bx + c = 0$ and they are

$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$

## 图像

### 默认

![Desktop View](/posts/20190808/mockup.png){: width="972" height="589" }
_图片的Caption_

## 视频

{% include embed/youtube.html id='Balreaj8Yqs' %}

## 交叉引用

[^footnote]: The footnote source
[^fn-nth-2]: The 2nd footnote source

## 例子
这里给出一个课程测评实例：
```markdown
---
title: [课程测评]摸鱼学导论
description: Meow
author: 通通
date: 2025-02-21 10:00:00 +0800
categories: [course_feedback, iai] 
tags: [course_feedback]
math: true
comments: true
---
# 课程内容
meow meow meow meow meow meow, meow meow meow meow.

1. meow.
2. meow meow, meow.
3. meow meow.

# 作业
meow meow, meow:

$$
\begin{equation}
    \mathrm{me}=\sup_{t}ow_t
\end{equation}
$$

# 成绩分布
> meow! meow meow, meow meow meow.
{: .prompt-danger }

```