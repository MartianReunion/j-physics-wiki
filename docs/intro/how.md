# 如何参与编写

在文章开始之前，**初中物理 Wiki** 项目组全体成员十分欢迎您为本项目贡献页面。正因为有了上百位像您一样的人，才有了 **初中物理 Wiki** 的明天！

这篇文章将主要叙述参与 **初中物理 Wiki** 编写的写作过程。请您在撰稿或者修正 Wiki 页面以前，仔细阅读以下内容，以帮助您完成更高质量的内容。

## 贡献指南
  
在开始编写一段内容之前，请查阅 [Issues](https://github.com/MartianReunion/j-physics-wiki/issues)，确认没有别人在做相同的工作之后，开个 [新 issue](https://github.com/MartianReunion/j-physics-wiki/issues/new) 记录待编写的内容。

在 Issues 中也有很多待修复 / 解决的问题，尤其是我们的BUG计划（Big Ugly Goose Plan）。从这里获取任务是一个很好的开始！

为了保证条目内容的专业性和准确性，我们建议您在编辑前先考虑以下几点：

1. **选择您熟悉的领域**：请优先编辑那些与您的专业知识、学习背景或兴趣爱好相关的条目。这有助于您创作出高质量的内容。
2. **谨慎对待新领域**：如果您对某个主题还处于初学阶段或不太了解，建议您先通过阅读、学习加深理解，待有一定把握后再动手编辑。
3. **查阅相关资料**：为条目添加内容或进行修订时，建议您先查阅权威文献和资料，确保信息准确无误。也欢迎您在页面评论区或我们的社区提出问题，与其他编者交流讨论。
4. **阅读我们的方针**：我们的方针中包含我们的理念与具体的一些规则，在阅读方针后进行编写，可以使你的内容更好地融入到初中物理Wiki中。你可以点击[这里](policy.md)查阅方针。

我们珍惜每位贡献者的热情和付出，也理解大家的专业水平不尽相同。让我们携手合作，共同呵护这个知识的乐园，用准确、专业的内容去帮助更多读者。期待您的贡献！在这里引用维基百科的一句话：

> 不要害怕编辑，勇于更新页面！

### 使用 Git 编辑

参与 **初中物理 Wiki** 的编写 **需要** 一个 GitHub 账号（可以前往 [GitHub 的账号注册页面](https://github.com/signup) 页面注册，但现在Github要双端验证，所以请参阅[这个教程](https://www.cnblogs.com/johnnyzen/p/17880870.html)），但 **不需要** 高超的 GitHub 技巧，即使你是一名新手，只要按照下面所述的步骤操作，也能够 **非常出色** 地完成编辑。这里我们推荐您[这个教程](https://oi-wiki.org/tools/git/)。

学会用git之后您就可以参与编辑了，具体流程如下。

1. 将主仓库 Fork 到自己的仓库中；
2. 将 Fork 后的分支仓库克隆（clone）到本地；
3. 在本地进行修改后提交（commit）这些更改；
4. 将这些更改推送（push）到你克隆的分支仓库；
5. 提交 Pull Request 至主仓库。

#### 向 Pull Request 追加更改

在 clone 下来的本地分支仓库中继续进行修改，并提交（commit）以及推送（push）这些更改即可。你的更改会被自动追加在 Pull Request 中。

!!! note "给管理员的特别提醒"

    为了保持内容的完整性与安全性，本仓库开启了`main`分支保护，虽然你可以直接写入仓库，但你必须通过PR向`main`分支添加内容。   
    **由于现阶段为开荒阶段，不启用保护措施。**

#### 预览变更

您在本地写好md文件就可以用 **vscode**或**typora**等软件预览变更。注意检查格式问题。

如果你的软件不能预览Mkdocs的一些扩展语法，或者你想预览页面部署后的状态，你可以参考[本地部署](#本地部署)这一节的内容。

#### 对于目录和引用的变更

通常情况下，如果您需要添加一个新页面，或者修改已有页面在目录中的链接，您就需要对 [`mkdocs.yml`](https://github.com/MartianReunion/j-physics-wiki/blob/main/mkdocs.yml) 文件作出改动。

添加新页面可以参考既有的格式。但除非是进行重构或修正名词，否则 **我们不建议对既有页面的引用链接进行修改**，Pull Requests 中不必要的修改也将被驳回。

#### Commit 信息格式规范

对于提交时需要填写的 commit 信息，请遵守以下几点基本要求：

1. commit 摘要请简要描述这一次 commit 改动的内容。注意 commit 摘要的长度不要太长。
2. 如果需要进一步描述本次 commit 内容，请在正文中详细说明。

对于 commit 摘要，请按照如下格式书写：

`<修改类型>(<文件名>或<可以描述更改的页面的文字内容>): <修改的内容>`

修改类型分为如下几类：

- `add`：用于添加内容的情况。
- `upd`：用于修正现有内容错误的情况。
- `ref`：用于对一个页面进行重构（较大规模的更改）的情况。
- `rol`：用于回退之前更改的情况。

#### Pull Request 信息格式规范

对于 Pull Request，请遵守以下几点要求：

1. 标题请写明本次 PR 的目的（做了 **什么** 工作，修复了 **什么** 问题）。
2. 内容请简要叙述修改的内容。如果修复了一个 issue 的问题，请在内容中添加 `repair #xxxx` 字段，其中 `xxxx` 代表 issue 的编号。

对于 Pull Request 的标题，推荐使用如下格式书写：

`<修改类型>(<文件名>或<可以描述更改的页面的文字内容>): <修改的内容> (<对应 issue 的编号>)`

修改类型与 Commit 一样。

示例：

- `add(mechanics/intro): 缝缝补补又三年`
- `upd(mechanics/gravity): 把重力的G写成F，已修改 (#1145)`
- `ref(electricity/ohms_law): 整理页面内容`
- `rol(electricity/intro): 写错了回滚一下`
- `add(欧姆定律): 编写了欧姆定律页面`

如果你的修改比较多或者杂，难以在标题中体现修改的名称，你可以使用`something`代替文件名，但你必须**仔细描述**你的修改内容。

例如：

- `upd(something): 修改了错别字(#1919)`

## Commit Recorder相关

本项目使用[CommitRecorder](https://github.com/BsoltB/CommitRecorder)来记录贡献者以及提交的文件。因此您在`git push`之前需要运行`commitrecord`来记录您的提交。

### 本地部署

本项目使用[Mkdocs](https://github.com/mkdocs/mkdocs)部署在[martianreunion.github.io/j-physics-wiki](https://martianreunion.github.io/j-physics-wiki/)。

为了能够在预览编辑后的**初中物理Wiki**，你可以在本地部署它。这需要你有Python3。

在克隆本项目后请使用

``` bash
pip install mkdocs-material
pip install mkdocs-ezlinks-plugin
pip3 install mkdocs-git-authors-plugin
```

安装必要的运行环境。

在此以后，你就可以通过以下命令启动一个运行在本地的服务器预览你的更改：

``` bash
mkdocs serve
```

在实际操作中，我们更推荐你在编辑过程中一直运行本地服务器。它会在你每一次保存文件后自动刷新页面，以便你随时查看最终的效果。

如果你有遇到一些问题，你可以阅读[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)的官方文档。

### 协作流程

请参考[方针](policy.md)中的编辑方针段落。
