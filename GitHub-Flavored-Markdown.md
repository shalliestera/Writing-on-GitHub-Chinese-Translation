Writing on GitHub / GitHub Flavored Markdown
[原文链接](https://help.github.com/articles/github-flavored-markdown/)
# GitHub 风格的 Markdown `GitHub Flavored Markdown` #
 Github 在站内问题、评论和合并请求上使用“GitHub风格的Markdown”（简称 GFM）。它在许多重要的方面与标准Markdown不同，并添加了一些额外功能。  
 如果你还不熟悉Markdown，先看一看 [Markdown基本语法]。如果你想了解更多关于疑问、评论和合并请求摘要中可用的特性，比如任务列表，请阅读 [writing on GitHub](#) 。
 
## 与传统 Markdown 的区别 ##
 
### 单词中的多重下划线 ###
Markdown 将下划线（`_`）转换成斜体，而 GFM 忽略单词中的下划线，如下：
> wow_great_stuff  
> do_this_and_do_that_and_another_thing.
这允许含有多个下划线的代码和名字正确地显示。强调单词的一部分，请使用星号（`*`）。
 
### URL 自动链接 ###
GFM 会自动链接标准 URL，因此如果你想链接到一个 URL（而不是设置链接文本），可以直接输入 URL，它会自动变成指向该 URL 的链接。
```markdown
http://example.com
```
变成
http://example.com
 
### 删除线 ###
GFM 添加了标准 Markdown 中缺少的给文本加删除线的语法。
```markdown
~~Mistaken text.~~
```
变成
~~Mistaken text.~~

### 包围起来的代码块 ###
 标准 Markdown 将每行行首以4个空格开头的文本转换为一个代码块；GFM 同样支持围起来的代码块。只需将你的代码用<code>```</code>包围，不需要用4个空格缩进。注意虽然fenced code blocks 不需要以空行开头——不像缩进代码块那样——我们仍推荐在代码前放置一个空行以使源 Markdown 代码更易于阅读。
<pre>
Here's an example:

```
function test() {
  console.log("notice the blank line before this function?");
}
```
</pre>
记住，在列表内，必须缩进8个空格以使  non-fenced code blocks 正确显示。

### 语法高亮 ###
代码块可以通过代码高亮更进一步。在你的 fenced block ，添加一个可选的语言标识符，可以产生语法高亮。举个例子，shshi使 Ruby 代码高亮：
```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```
我们使用 [Linguist](https://github.com/github/linguist) 来完成语言检测和语法高亮。你可以通过精读 [the languages YAML file](https://github.com/github/linguist/blob/master/lib/linguist/languages.yml) 了解哪些关键词有效。

### 表格 ###
通过组合一个单词表，并用连字符（`-`）分隔第一行，用竖线（`|`）分隔每一列，来创建表格：
```markdown
First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell
```
为求美观，可以在末尾添加额外的竖线：
```markdown
| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |
```
注意，最上面的连字符的长度并不需要和表头文字的长度相同：
```markdown
| Name | Description          |
| ------------- | ----------- |
| Help      | Display the help window.|
| Close     | Closes a window     |
```
可以包含其他 Markdown 代码如 链接、斜体或删除线：
```markdown
| Name | Description          |
| ------------- | ----------- |
| Help      | ~~Display the~~ help window.|
| Close     | _Closes_ a window     |
```
最后，在表头行添加冒号（`:`），可以定义文本为左对齐、右对齐还是居中对齐：
```markdown
| Left-Aligned  | Center Aligned  | Right Aligned |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |
```
最左端的冒号指明此列左对齐；最右端的冒号指明此列右对齐；两段都有冒号指明此列居中对齐。

## HTML ##
可以在你的 README 、疑问和合并请求中使用 HTML 的子集。  
我们支持的标签和属性的完整列表在  [github/markup repository]( github/markup repository) 。

### 延伸阅读 ###
"[Writing on GitHub]()"
