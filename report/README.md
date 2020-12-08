# hw3 report

|||
|-:|:-|
|Name|林佑檍|
|ID|0711099|

## How much time did you spend on this project

e.g. 4 whole days.

## Project overview

Describe the project structure and how you implemented it.

### Scanner.l
1. 增加回傳值
    - 利用 yylval 回傳 token 的值

### Parser.y
1. 增加型別描述
    - 在%union中增加其他型別供scanner回傳
    - 宣告nonterminal的回傳型別, e.g. %type <node> Declaration
2. 在grammer rule中加入action
    - action預設為$$=$1, 但幾乎都要修改或增加

### AST
- 其他 Node 皆繼承自 AstNode
- 定義好 Node 後透過 parser內的 action 完成整個AST

## What is the hardest you think in this project

老實時說每個地方對我來說都很困難, 每個Node該怎麼建, 裡面該存甚麼資料, 怎麼存, parser內的action該怎麼寫我都要花很多間研究才能寫出一點點, 最後結果就是整個都寫不出來, 只能祈禱作業四跟五寫得出來

## Feedback to T.A.s

畢竟寫不出來, 所以也不知道有什麼地方可以改進
