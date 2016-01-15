Writing on GitHub / Markdown Basics  
[本页原文](https://help.github.com/articles/markdown-basics/)
# Markdown 基础语法 #

[Markdown](http://daringfireball.net/projects/markdown/) 允许你使用`易于阅读`，`易于书写`的纯文本格式写作，随后可转换成在 GitHub 上查看的有效的 HTML。

## 写作基础 ##

### 段落 ###
Markdown 中的段落是紧接着若干空行的数行连续文本。
```Markdown
On July 2, an alien mothership entered Earth's orbit and deployed several dozen saucer-shaped "destroyer" spacecraft, each 15 miles (24 km) wide.

On July 3, the Black Knights, a squadron of Marine Corps F/A-18 Hornets, participated in an assault on a destroyer near the city of Los Angeles.
```

### 标题 ###
你可以通过在标题文本前添加一个或多个 `#` 号来创建标题。`#` 号的数量决定标题的大小。
```Markdown
# The largest heading (an <h1> tag)
## The second largest heading (an <h2> tag)
…
###### The 6th largest heading (an <h6> tag)
```
### 引用 `Blockquotes` ###
你可以用一个 `>` 号表明 [blockquotes](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/blockquote) 。
```Markdown
In the words of Abraham Lincoln:

> Pardon my french
```

### 带样式的文本 `Styling text` ###
可以使文本 **[加粗](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/strong)** 或 *[倾斜](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/em)* 。
```markdown
*This text will be italic*
**This text will be bold**
```
**加粗** 或 *倾斜* 既可以使用 `*` 包围需要样式的文本也可以使用 `_` 。这允许你在需要时同时使用粗体和斜体。
```markdown
**Everyone _must_ attend the meeting at 5 o'clock today.**
```

## 列表 ##

### 无序列表 ###
在列表项前面加一个 `*` 或者 `-` 来创建一个 [无序列表](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul) 。
```markdown
* Item
* Item
* Item

- Item
- Item
- Item
```

### 有序列表 ###
在列表项前面添加一个 `数字` 来创建 [有序列表](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul) 。
```markdown
1. Item 1
2. Item 2
3. Item 3
```

### 嵌套列表 ###
在列表项前面缩进2个空格，可以创建嵌套列表。
```markdown
1. Item 1
  1. A corollary to the above item.
  2. Yet another point to consider.
2. Item 2
  * A corollary that does not need to be ordered.
    * This is indented four spaces, because it's two spaces further than the item above.
    * You might want to consider making a new list.
3. Item 3
```

## 代码格式化 ##

### 内联格式 ###
使用一对重音符 （`` ` ``）让文本变成特殊的等宽字体格式。所有在这对重音符内的文本会原样显示，不带其他格式。
```markdown
Here's an idea: why don't we take `SuperiorProject` and turn it into `**Reasonable**Project`.
```

### 多行代码 ###
三个重音符 （<code>```</code>）使文本单独成块显示。
<pre>
Check out this neat program I wrote: 

```
x = 0
x = 2 + 2
what is x
```
</pre>

## 链接 ##
用一对方括号 （`[ ]`）括住链接文本，然后用一对圆括号 （`( )`） 括住链接本身，来创建一个内联链接。  
例如，创建一个跳转到 [www.github.com](http://www.github.com/) 的超链接，链接文本是“Visit GitHub!”，用 Markdown 是这么写的： `[visit GitHub!](http://www.github.com)` 。

## 另请参阅 ##
* [GitHub Flavored Markdown](#)
* [Writing on GitHub](#)
* [Mastering Markdown](#)
