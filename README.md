
# 英文书籍翻译小组用户手册

* [翻译计划](#翻译计划)
* [翻译过程](#翻译过程)


## 翻译计划


* 注册 github.com 帐号并建立 [项目 github 仓库](https://github.com/HackTec/)
* 召集小伙伴:@ibrother、@ChanZou、@ieted、@kingname、@Mangosteen-Yang
* 建立微信协作群，及时沟通与交流翻译过程中遇到的各类问题

接下来就是这里的用户手册编写，到这里要做的工作是：

* 更详细地描述翻译和提交过程，简化大家的参与过程

* 制定文档格式规范

* 理清一些基本的翻译约定


## 翻译过程

* 注册并登录 github fork [代码仓库](https://github.com/HackTec/HT-zh-books-translation)

* 注册 gitbook.com，在 gitbook.com 建立书籍并绑定到 github.com 刚 fork 的仓库。

* clone 代码仓库

        git clone git@github.com:HackTec/HT-zh-books-translation.git

* 找到自己选择的部分，进行翻译。

* 开始翻译

    * 翻译时可以用markdown编辑器。
    * 也可以用本地的工具，如 vim 编辑

* 翻译时

    * 请尽量遵守英文原稿的格式
    * 请规范使用 [Markdown 语法][markdown]
    * 英文和数字短语前后须加空格，以便获得更好的视觉感受
    * 代码片段上下须加空行，代码片段可以用 \`\`\` 前后括起来，请参考[Markdown][markdown] `Code and Syntax Highlighting` 一节。
    * --target 和 --host 之类的命令或者参数最好用标示符 \` 括起来。效果如：`--target` 和 `--host`
    * 全篇要统一用中文标点符号，全部用全角。
    * 碰到专业名词，特定缩写，不需要翻译。
    * 所有目录的标题中的 `Contents` 翻译为 `目录`。
    * 不保留英文原文，只保留中文译文。
    * 每翻译完一个段落请务必通读
        * 确保用词没有歧义，整段衔接流畅，如有必要请调整/添加必要的衔接词汇
        * 并对照英文原文确保没有漏掉原文任何需要表达的含义，不要刻意漏掉部分自己感觉模糊的词汇
    * 如果有部分段落或者词汇理解模糊，请优先在协作群讨论或者借助第三方翻译工具协助，推荐 bing.com, iciba.com


* 及时同步远程 master 分支并 rebase develop 到 master 上

        git checkout master && git pull
        git rebase --onto master --root

