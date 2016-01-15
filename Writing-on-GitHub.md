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

### ###
