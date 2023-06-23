<div align="center">
  <h3>🎉 2023毕业快乐 🎉</h3>
  <p>祝各位一切顺利! 🎓🎉🎊🥳</p>
  <img src="https://p7.itc.cn/q_70/images03/20230621/4f87443856da41819fbfc6372342e5b5.jpeg" alt="Graduation image">
</div>

# SJTU 2023本科生毕业论文模板


该模板改自sjtug的官方[SJTUThesis](https://github.com/sjtug/SJTUThesis)模板。参考了[2023年最新版规定](04-2023-05-30-2023年本科生毕业论文形式规范解读.pdf)做了下述更改。如果有更多的问题，欢迎反馈到官方的[issues](https://github.com/sjtug/SJTUThesis/issues)或此repo。

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

4. 中文封面仅有年月，英文封面年月日。🤔🤨

    `setup.tex`注释第74行。

### 目录

1. 添加摘要和ABSTRACT。

    添加`\addcontentsline{toc}{chapter}{摘要}`以及`\addcontentsline{toc}{chapter}{ABSTRACT}`。详见discussion [#942](https://github.com/sjtug/SJTUThesis/discussions/942).

2. 缩进。
    感谢水源大佬的[帖子](https://shuiyuan.sjtu.edu.cn/t/topic/166804).

    根据学校要求：
    >章目录：宋体四号,单倍行距，页码右对齐。
    >小节目录：宋体小四号，单倍行距，左缩进1个汉字符，两端对齐，页码右对齐。
    >二级小节目录：宋体五号,单倍行距，左缩进2个汉字符，两端对齐，页码右对齐。

    添加：
    ```latex
    \setlength{\cftsecindent}{1em}
    \setlength{\cftsubsecindent}{2em}
    ```

### 参考文献

1. 参考文献题目格式需修改为“黑体，加粗，三号，居中，每字空一格”。

    在`setup.tex`96行编辑`bib = {参\hspace{\ccwd}考\hspace{\ccwd}文\hspace{\ccwd}献},`

## 致谢

感谢maintainer [LogCreative](https://github.com/LogCreative)的细心答复。

感谢水源大佬[蝉时雨的帖子](https://shuiyuan.sjtu.edu.cn/t/topic/166804).

感谢[Megumism](https://github.com/Megumism)，[pixas](https://github.com/pixas)在提出的问题。
