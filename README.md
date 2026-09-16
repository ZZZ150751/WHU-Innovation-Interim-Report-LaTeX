# 武汉大学大学生创新创业训练计划项目中期报告 LaTeX 模板

一个适用于 **武汉大学大学生创新创业训练计划项目中期报告** 的 LaTeX 模板。

本模板根据本人实际使用的中期报告整理，希望能给后面的武大学弟学妹省一点排版时间。

> **注意：** 本模板为个人整理的非官方模板，仅供参考。不同学院、不同年份的中期检查要求可能发生变化，请以当年学院或学校发布的最新通知为准。

---

## 文件结构

```text
.
├── main.tex
├── example.pdf
├── figure/
└── README.md
```

其中：

* `main.tex`：LaTeX 主文件
* `example.pdf`：模板编译后的示例 PDF
* `figure/`：存放正文图片
* `README.md`：项目说明

---

## 使用方法

推荐使用 **XeLaTeX** 编译。

如果使用 Overleaf：

1. 新建一个空白项目；
2. 上传 `main.tex`；
3. 将 Compiler 设置为 `XeLaTeX`；
4. 修改项目基本信息；
5. 按正文中的提示填写内容；
6. 编译即可。

如果在本地使用 TeX Live 等环境，可以执行：

```bash
xelatex main.tex
xelatex main.tex
```

建议编译两次，以正确生成目录、公式编号和交叉引用。

---

## 修改项目信息

一般只需要修改 `main.tex` 开头定义的基本信息：

```latex
\newcommand{\ProjectNumber}{20XX10486XXX}

\newcommand{\ProjectTitleCN}{在此填写项目中文名称}

\newcommand{\CollegeCN}{XX学院}

\newcommand{\MajorCN}{XX专业}

\newcommand{\StudentNamesCN}{张三、李四、王五}

\newcommand{\AdvisorCN}{XX教授}
```

修改完成后，再按照正文中的提示逐项填写即可。

---

## 图片

建议在项目目录下建立：

```text
figure/
```

文件夹，并将所有图片统一放在其中，例如：

```text
figure/
├── framework.png
├── experiment.png
└── result.png
```

正文中可以使用：

```latex
\begin{figure}[htbp]
    \centering
    \includegraphics[width=0.8\textwidth]{figure/result.png}
    \caption{实验结果}
    \label{fig:result}
\end{figure}
```

并通过：

```latex
如图~\ref{fig:result} 所示。
```

进行引用。

模板中的示例图片可以使用空白框，因此仓库刚 clone 下来时无需额外准备图片即可编译。

---

## 正文结构

模板目前包括：

```text
封面
英文扉页
声明
中文摘要
英文摘要
目录

第1章 绪论
    1.1 研究背景
    1.2 研究意义
    1.3 研究内容
    1.4 研究方法

第2章 模型与算法

第3章 数值实验与结果分析

第4章 项目进度与后续计划
    4.1 项目完成情况
    4.2 目前存在的问题
    4.3 下一阶段计划

参考文献
```

正文中保留了简单的填写提示，可以根据实际项目自由增删章节。

---

## 说明

本模板为个人整理的 **非官方模板**，仅供参考。

不同学院、不同年份的中期检查要求可能发生变化，请以当年学院或学校发布的最新通知为准。

如果学校或学院发布了新的 Word / PDF 格式要求，建议重点核对：

* 页边距
* 中文及英文字体
* 字号
* 行距
* 封面格式
* 项目编号格式
* 签字页要求
* 摘要及关键词格式
* 参考文献格式

若官方要求与本模板存在冲突，请以官方要求为准。

---

## Contribution

如果你发现格式问题，或者某一届学校要求发生变化，欢迎提交 **Issue** 或 **Pull Request**。

如果这个模板对你有帮助，也欢迎点一个 ⭐ Star。

---

## Disclaimer

本项目与武汉大学官方无关，仅为个人整理并公开分享。

模板中涉及的学校名称仅用于说明模板适用场景，具体格式要求请以武汉大学及相关学院当年发布的官方通知为准。
