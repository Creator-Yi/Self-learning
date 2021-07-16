---
weight: 4
title: "Markdown 基本语法"
date: 2021-07-04T22:51:22+08:00
tags: ["Markdown"]
---
---
自己写来熟悉一下Markdown的语法


***



## markdown标题
从`H2`到`H6`标题在每个级别上加上一个`#`

```markdown
## h2 标题
### h3 标题
#### h4 标题
##### h5 标题
###### h6 标题
```
输入出如下

## h2 标题
### h3 标题
#### h4 标题
##### h5 标题
###### h6 标题

如果你想添加自定义标题ID，在标题后面加花括{}

```markdown
### 一个带ID的标题{#ID}
```

## 注释 
markdown 的注释和html 注释相兼容
```HTML
<!--
    注释
-->
```
<!--
    注释
-->
⬆️⬆️⬆️注释看不到o！

## 水平线

Markdown可以使多种方法：
* `___`：三个下划线
* `---`：三个破折号
* `***`：三个星号

输出的效果如下：

___
---
***

## 段落与内联
Markdown的段落是纯文本的，这就是一个段落

而HTML里是需要用`<p></p>`来包裹的

如果你需要HTML的标签，可以这样使用：
```html
Markdown 格式的段落
<div class="class">
    这是<b>HTML</b>
</div>
```

### 加粗

以下文本会被 **加粗**
```markdown
**渲染成粗体**
__渲染成粗体__
```

### 斜体

以下文本片段被 _渲染为斜体_
```markdown
*渲染成斜体*
_渲染成斜体_
```

### 删除线

```markdown
~~这是删除了的文本~~
```

输出如下

~~这是删除了的文本~~

### 组合

加粗，斜体，删除线可以组合使用
```markdown
***加粗和斜体***
~~**删除线和加粗**~~
~~*删除线和斜体*~~
~~***加粗, 斜体和删除线***~~
```
输出如下

***加粗和斜体***

~~**删除线和加粗**~~

~~*删除线和斜体*~~

~~***加粗, 斜体和删除线***~~

## 引用

在文档中引用其他来源的内容

在要引用的文本前添加`>`

```markdown
>**人月神话**所有的编程人员都是乐观主义者。可能是这种现代魔术特别吸引那些相信美满结局的人；
也可能是成百上千琐碎的挫折赶走了大多数人，只剩下了那些习惯上只关注结果的人；
还可能仅仅因为计算机还很年轻，程序员更加年轻，而年轻人总是些乐观主义者——无论是什么样的程序，
结果是勿庸置疑的：“这次它肯定会运行。”或者“我刚刚找出了最后一个错误。”
```

输出如下

>**人月神话**所有的编程人员都是乐观主义者。可能是这种现代魔术特别吸引那些相信美满结局的人；
也可能是成百上千琐碎的挫折赶走了大多数人，只剩下了那些习惯上只关注结果的人；
还可能仅仅因为计算机还很年轻，程序员更加年轻，而年轻人总是些乐观主义者——无论是什么样的程序，
结果是勿庸置疑的：“这次它肯定会运行。”或者“我刚刚找出了最后一个错误。”

引用也可以嵌套:

```markdown
> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue.
Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
>> Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor
odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.
```

输出如下

> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue.
Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
>> Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor
odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.

## 列表

### 无序列表

你可以使用以下任意符号来组成无序列表中的项：

```markdown
* 一项内容
+ 一项内容
- 一项内容
```


```markdown
* 一项内容
* 一项内容
* 一项内容
* 一项内容
* 一项内容
  * 附属内容
  * 附属内容
  * 附属内容
  * 附属内容
* 一项内容
* 一项内容
* 一项内容
```

输出如下

* 一项内容
* 一项内容
* 一项内容
* 一项内容
* 一项内容
  * 附属内容
  * 附属内容
  * 附属内容
  * 附属内容
* 一项内容
* 一项内容
* 一项内容

### 有序列表

```markdown
1. 焦油坑
2. 人月神话
3. 外科手术队伍
4. 贵族专制、民主政治和系统设计
```
输出如下

1. 焦油坑
2. 人月神话
3. 外科手术队伍
4. 贵族专制、民主政治和系统设计

{{< admonition tip >}}
如果你对每一项使用 `1.`, Markdown 将自动为每一项编号. 例如:


```markdown
1. 焦油坑
1. 人月神话
1. 外科手术队伍
1. 贵族专制、民主政治和系统设计
```
输出如下

1. 焦油坑
1. 人月神话
1. 外科手术队伍
1. 贵族专制、民主政治和系统设计
{{< /admonition >}}

### 任务列表

任务列表使你可以创建带有复选框的列表.
要创建任务列表, 请在任务列表项之前添加破折号 (`-`) 和带有空格的方括号 (`[ ]`). 要选择一个复选框，请在方括号之间添加 x (`[x]`).

```markdown
- [x] 打游戏
- [ ] 不打游戏
- [ ] 去学习
```

输出如下

- [x] 打游戏
- [ ] 不打游戏
- [ ] 去学习  
  
## 代码

### 行内代码

用 <code>`</code> 包装行内代码段.

```markdown
在这个例子中, `<section></section>` 会被包裹成 **代码**.
```

呈现的输出效果如下:

在这个例子中, `<section></section>` 会被包裹成 **代码**.

### 高亮语法


要激活它，只需在第一个代码 "围栏" 之后直接添加你要使用的语言的文件扩展名,
<code>```js</code>, 语法高亮显示将自动应用于渲染的 HTML 中.

例如, 在以下 JavaScript 代码中应用语法高亮:


{{< highlight markdown >}}
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
{{< / highlight >}}

输出效果如下

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

{{< admonition >}}
**Hugo** 文档中的 [语法高亮页面](https://gohugo.io/content-management/syntax-highlighting/) 介绍了有关语法高亮的更多信息,
包括语法高亮的 shortcode.
{{< /admonition >}}

## 10 表格

通过在每个单元格之间添加竖线作为分隔线, 并在标题下添加一行破折号 (也由竖线分隔) 来创建表格. 注意, 竖线不需要垂直对齐.

```markdown
| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |
```

呈现的输出效果如下:

| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

{{< admonition note "文本右对齐或居中对齐" >}}
在任何标题下方的破折号右侧添加冒号将使该列的文本右对齐.

在任何标题下方的破折号两边添加冒号将使该列的对齐文本居中.

```markdown
| Option | Description |
|:------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |
```

呈现的输出效果如下:

| Option | Description |
|:------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |
{{< /admonition >}}

## 链接 {#link}

### 基本链接

```markdown
<https://baidu.com>
<contact@revolunet.com>
[必应](https://bing.com)
```

输出如下 （鼠标停留链接上，没有提示）

<https://baidu.com>

<contact@revolunet.com>

[必应](https://bing.com)

### 添加一个标题

```markdown
[百度](https://bing.com "这是必应哒！")
```
输出效果如下 (将鼠标悬停在链接上，会有一行提示):

[百度](https://bing.com "这是必应哒！")


### 定位标记

定位标记使你可以跳至同一页面上的指定锚点. 例如, 每个章节:

```markdown
## Table of Contents
  * [Chapter 1](#chapter-1)
  * [Chapter 2](#chapter-2)
  * [Chapter 3](#chapter-3)
```

将跳转到这些部分:

```markdown
## Chapter 1 <a id="chapter-1"></a>
Content for chapter one.

## Chapter 2 <a id="chapter-2"></a>
Content for chapter one.

## Chapter 3 <a id="chapter-3"></a>
Content for chapter one.
```

{{< admonition >}}
定位标记的位置几乎是任意的. 因为它们并不引人注目, 所以它们通常被放在同一行了.
{{< /admonition >}}



## 12 脚注

脚注使你可以添加注释和参考, 而不会使文档正文混乱.
当你创建脚注时, 会在添加脚注引用的位置出现带有链接的上标编号.
读者可以单击链接以跳至页面底部的脚注内容.

要创建脚注引用, 请在方括号中添加插入符号和标识符 (`[^1]`).
标识符可以是数字或单词, 但不能包含空格或制表符.
标识符仅将脚注引用与脚注本身相关联 - 在脚注输出中, 脚注按顺序编号.

在中括号内使用插入符号和数字以及用冒号和文本来添加脚注内容 (`[^1]：这是一段脚注`).
你不一定要在文档末尾添加脚注. 可以将它们放在除列表, 引用和表格等元素之外的任何位置.

```markdown
这是一个数字脚注[^1].
这是一个带标签的脚注[^label]

[^1]: 这是一个数字脚注
[^label]: 这是一个带标签的脚注
```

这是一个数字脚注[^1].

这是一个带标签的脚注[^label]

[^1]: 这是一个数字脚注
[^label]: 这是一个带标签的脚注

## 13 图片

图片的语法与链接相似, 但包含一个在前面的感叹号.

```markdown
![Minion](https://octodex.github.com/images/minion.png)
```

![Minion](https://octodex.github.com/images/minion.png)

或者:

```markdown
![Alt text](https://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")
```

![Alt text](https://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")

像链接一样, 图片也具有脚注样式的语法:

```markdown
![Alt text][id]
```

![Alt text][id]

稍后在文档中提供参考内容, 用来定义 URL 的位置:

```markdown
[id]: https://octodex.github.com/images/dojocat.jpg  "The Dojocat"
```

[id]: https://octodex.github.com/images/dojocat.jpg  "The Dojocat"
