# 初中物理Wiki

**物理学**是以实验为基础，研究力、热、声、光、电等物理现象的自然科学。

在初中阶段，物理学培养学生的科学思维和对基本物理概念的直观理解。通常，我国的中学会在初二时引入物理课程，并将其作为中考的关键科目之一。无论是为了考试，还是为了提升思维能力与个人素质，学习物理都是必要的。

为了使广大中学生能更好地学习物理知识，我们参照[OI Wiki](https://oi-wiki.org/)，创立此站点。

目前，本wiki整出于**开荒阶段**，需要各位的帮助。如果你对这个项目感兴趣，欢迎参与！

我们源于社区，提倡**知识自由**，在未来也绝不会商业化，将始终保持独立自由的性质。

## 版权声明

[![知识共享许可协议](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](https://gitee.com/link?target=https%3A%2F%2Fcreativecommons.org%2Flicenses%2Fby-sa%2F4.0%2F)  
除特别注明外，项目中除了代码部分均采用[(Creative Commons BY-SA 4.0) 知识共享署名 - 相同方式共享 4.0 国际许可协议](https://gitee.com/link?target=https%3A%2F%2Fcreativecommons.org%2Flicenses%2Fby-sa%2F4.0%2Fdeed.zh)及附加的 [The Star And Thank Author License](https://github.com/zTrix/sata-license) 进行许可。

换言之，使用过程中您可以自由地共享、演绎，但是必须署名、以相同方式共享、分享时没有附加限制，

而且应该为 GitHub 仓库点赞（Star）。

## 本地部署

本站点基于网络，但也可以本地部署。但这要求你有Python3和pip环境以及git。

1. 克隆本仓库

    ``` bash
    git clone https://github.com/MartianReunion/j-physics-wiki.git
    ```

2. 安装依赖

    ``` bash
    pip install mkdocs-material #安装mkdocs以及material主题
    
    #安装使用的插件
    pip install mkdocs-ezlinks-plugin
    ```

3. 运行或部署

    如果你希望直接运行，你可以使用下述命令。它允许你实时预览更改。

    ``` bash
    mkdocs serve
    ```

    如果你希望把页面编译为一个静态的网页，你可以使用下述命令。这允许你直接通过静态http服务器运行，但你不能通过它预览更改。

    ``` bash
    mkdocs build
    ```

4. 获取更新（可选）

    本地的仓库可能过时，可以使用下述命令同步远程仓库。

    ``` bash
    git pull
    ```
