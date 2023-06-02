# SJTU 本科生毕业论文模板

该模板改自sjtug的官方[SJTUThesis](https://github.com/sjtug/SJTUThesis)模板。参考了[最新版规定](04-2023-05-30-2023年本科生毕业论文形式规范解读.pdf)做了下列更改。

## 更改

### 主体

1. 单页打印。

    `main.tex`中添加`oneside`设置。

2. 摘要、英文摘要、目录、英文大摘要的页眉不需要表明。

    详见issue [#953](https://github.com/sjtug/SJTUThesis/discussions/953)

### 封面

参考issue [#941](https://github.com/sjtug/SJTUThesis/issues/941)

1. 修改“上海交通大学学士学位论文”为“上海交通大学学位论文”。

    注释`sjtu-lang-thesis-zh.def`第37行。

2. 更改“学科/专业”为“学科 / 专业名称”。

    修改`sjtu-name-thesis-zh.def`第51行。
    修改`sjtu-lang-thesis-zh.def`第118行的宽度。

3. 增加“申请学位层次”。

    注释`sjtu-lang-thesis-zh.def`第114行。
    修改`sjtu-name-thesis-zh.def`第52行。

### 目录

1. 添加摘要和ABSTRACT。

    添加`\addcontentsline{toc}{chapter}{摘要}`以及`\addcontentsline{toc}{chapter}{ABSTRACT}`。详见discussion [#942](https://github.com/sjtug/SJTUThesis/discussions/942).