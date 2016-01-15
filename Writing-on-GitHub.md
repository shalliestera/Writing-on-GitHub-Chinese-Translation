Writing on GitHub / Writing on GitHub
# 在 GitHub 上写作 #
isusues、评论和合并请求描述由 GibHub 风格的 Markdown 写成，其中含有使得在GitHub上更易于写作的额外特性。

## 标记 ##

### 换行 ###
在 GitHub 上写作的最大不同是处理换行的方式。当使用 Markdown 时，你可以用硬换行将文本弄成单独一行。我们发现这样会引发大量无心的格式化错误。在评论中，GitHub 像你通常期望地将“类似段落的内容”作为新行一样换行。  
下面的段落包含由单个换行符分隔的两个短语：
```markdown
Roses are red
Violets are blue
```
变成
Roses are red  
Violets are blue

### 任务列表 ###
列表可以通过在前面添加 `[ ]` 或 `[x]` （分表代表`未完成`和`已完成`），转变成[任务列表]()。
```markdown
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> are supported
- [x] list syntax is required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
```
带复选框的任务列表可以在所有 comments 和 Markdown 文件中显示。整个 GitHub 上都支持通过选中、未选中复选框来标记已完成或未完成。  
任务列表可以嵌套以更好地构造你的任务：
```markdown
- [ ] a bigger project
  - [ ] first subtask #1234
  - [ ] follow up subtask #4321
  - [ ] final subtask cc @mention
- [ ] a separate task
```
任务列表可以嵌套至任意深度，然而我们推荐嵌套最多一两次；更复杂的任务应当分解成单独的列表。

### References ###
Certain references 自动链接：
```markdown
* SHA: a5c3785ed8d6a35868bc169f07e40e889087fd2e
* User@SHA: jlord@a5c3785ed8d6a35868bc169f07e40e889087fd2e
* User/Repository@SHA: jlord/sheetsee.js@a5c3785ed8d6a35868bc169f07e40e889087fd2e
* #Num: #26
* GH-Num: GH-26
* User#Num: jlord#26
* User/Repository#Num: jlord/sheetsee.js#26
```
变成
* SHA: a5c3785ed8d6a35868bc169f07e40e889087fd2e
* User@SHA: jlord@a5c3785ed8d6a35868bc169f07e40e889087fd2e
* User/Repository@SHA: jlord/sheetsee.js@a5c3785ed8d6a35868bc169f07e40e889087fd2e
* #Num: #26
* GH-Num: GH-26
* User#Num: jlord#26
* User/Repository#Num: jlord/sheetsee.js#26

## 特性 ##

### 快速引用 ###
键入你键盘上的 `r` 让你回复当前 issue 或 带评论的合并请求。在讨论帖中选中任意文本，按 `r`，将自动以块引用的格式添加到你的评论中。

### 名字和 Team @提醒 自动完成 ###
输入一个 `@` 符号会弹出一个 project 里的 人或 team 的列表。这个列表随你的输入而过滤，所以当你找到你想找的人名或 team 名，可以用方向键选择然后按 tab 键或 enter 键来补全名字。举个例子，只需要键入 @组织/team名 ，所有 team 成员都将订阅到 issue。

自动补全的结果限定为仓库协作者和帖子的其他参与者，因此不是完整的全局搜索。它使用如文件查找一般的模糊过滤器，通过用户名和全名起作用。

更多关于 @提醒 [用户](https://github.com/blog/1004-mention-autocompletion) 和 [teams](https://github.com/blog/1121-introducing-team-mentions) 的自动完成的信息，请查阅博客帖子。

### 颜文字自动补全 ###
键入 `:` 会弹出一个颜文字建议列表。这个列表随着你的输入而过滤，因此当你找到所需的颜文字时，按 **Tab** 或 **Enter ** 补全高亮结果。可用的颜文字完整列表，请查阅 [emoji-cheat-sheet.com](http://emoji-cheat-sheet.com/)。

### Issue 自动补全 ###
键入 `#` 会弹出一个建议的 Issues 和 Pull Requests 的列表。键入一个数字或一些文本以过滤列表，然后按 `Tab` 或 `Enter` 补全高亮的结果。

## 另请参阅 ##

[Markdown Basics]()
[GitHub Flavored Markdown]()
