# Latex Writing

## 写作中
一般来说,方法应该先写,再做实验,最后写引言摘要

个人认为只有非常懂文章的三个新颖贡献才能最开始写引言

### 摘要写作逻辑(五段论)
- 做的是什么？
- 应用在哪？
- 之前方法存在什么问题？
- 这篇文章使用了什么技术解决这个问题？
- 效果如何？

### 引言写作逻辑
- 做的是什么(大概背景)
- 之前方法为什么不行？&& 挑战点在哪？
- 如何解决这些挑战的？Insight和Intuition要讲明白
- 本文贡献点：新问题、新方法、理论保障、丰富的实验

### 全文写作逻辑
- 新手写作时刻要遵循总分逻辑去写作,这样能确保逻辑连贯,即首先介绍这一章大致内容(即每小节的内容的概括),然后再分开讲述每小节内容
- 如果上一句的主语和当前主语不一致,则需要连接词使逻辑顺畅
    - **表示转折**: although, however, on the contrary, in spite of, yet, despite, but, nevertheless, otherwise, unfortunately, albeit
    - **表示并列**: and, more than that, likewise, in addition, for instance/example, also, moreover, furthermore, what is more, intuitively, a, concretely, specifically, empirically, specially, first/second/lastly
    - **表示因果**: as a result, because, thus, so, as, since, therefore, consequently, on account of, ultimately
    - **表示归纳**: as a result, finally, therefore, thus, accordingly, in short, consequently, in conclusion, so, in a word, in brief, certainly, in a nutshell, overall
- 分点让逻辑更清晰
    - Our technique can improve XXX for three reasons. First, xxx. Second, xxx. Third, xxx.
    - We investigate such xxx and discover three reasons: (1) xxx; (2) xxx; and (3) xxx.
- 理由要精炼得体,下列语句是摘抄自A类文章,[更多摘抄语句](sentences.txt)
    - Since xx is not open-source, we implement xx from scratch faithfully following the original design principles, as well as caching the top-level nodes on compute nodes for better performance.
    - Since then, both the hardware and workload landscapes have changed.

### 公式
- 数学符号: [A short list of commonly used LATEX symbols](https://artofproblemsolving.com/wiki/index.php/LaTeX:Symbols)
- 公式如果太长,可以用`\hsapce{-0.1em}`或者在两个符号中间加`\!`
- 需编号,**结尾有标点**(下文接where用逗号,没有则用句号),不超宽,等号对齐

### 图表(通常放在论文最顶/底端)
- 算法. 建议使用[algorithm2e package](https://www.ctan.org/pkg/algorithm2e)
- 图片, 见[画图项目](https://github.com/Josehokec/python_figure).
- 表格. 初学者生成表格可以参考[Tables Generator](https://www.tablesgenerator.com)和[Latex-tables](https://www.latex-tables.com)

注意：图标字体统一，字号不大于正文、也不宜过小，标题、图例和坐标轴表达清楚，配色美观

```
\begin{table}
\caption{Comparison of average query latency under different evaluation engines on Crimes and Citibike datasets.}
\addvspace{-1em}
\label{tab:engine_latency}
\centering
\scalebox{0.7}{
\begin{tblr}{
  rowsep=0.8pt,                 % 设置行间距
  cell{1}{1} = {r=2}{},         % 第1行第1列跨2行
  cell{1}{2} = {c=3}{c},        % 第1行第2列跨3列
  cell{1}{5} = {c=3}{c},        % 第1行第5列跨3列
  vline{1, 2, 5, 8} = {1-6}{},  % 在第1-4行，第2和第6列前加垂线
  hline{1,3,7} = {-}{},         % 在第1、3、8行画水平线。
  hline{2} = {2-7}{},           % 水平线画到第2到7列
}
{\bf Approaches}    &{\bf Crimes Dataset}&& & {\bf Citibike Dataset} &     \\
 &{\bf Our SASE}    &{\bf Esper}&{\bf Flink}& {\bf Our SASE}& {\bf Esper}  & \textbf{Flink} \\
\textbf{DFS (Ours)} &{\bf0.68s} &{\bf1.09s} &{\bf5.56s}     &{\bf 0.97s}   & {\bf 1.35s} & {\bf2.68s}\\
\textbf{Pushpull}   & 1.74s     & 2.22s     & 7.80s         & 1.46s & 1.81s & 4.75s\\
\textbf{Pushdown+}  & 0.96s     & 1.72s     & 14.07s        & 2.10s   & 2.70s & 59.61s\\
\textbf{Pushdown}   & 1.44s     & 3.20s     & 34.04s        & 2.25s   & 2.91s & 68.96s
\end{tblr}
}
\end{table}
```
<center class ='img'>
<img title="bar_example" src="table_example.png" width="40%">
</center>  


### 排版
- 标题和子标题单词首字母大写(介词除外)
- 如果首行字体加粗了,后续内容不应该出现加粗,用下划线或者斜体替代
- 下划线推荐使用`\usepackage[normalem]{ulem}`,normalem参数能避免给参考文献加下划线

### 引用格式
- 正常来说,去掉引用不应该影响句子的完整性,此外一般我喜欢在引用前加波浪线,如`~\cite{Paper1}`
- 在[dblp](https://dblp.org/)上去寻找获取论文BibTeX,注意:每年论文导入的Bib风格不一样,需要自己修改统一,如会议是否缩写、会议地点、出版社名
- 标题中需要强制大小写的单词用 {...} 括起来，例如 {RDF}、{DBpedia}
- 个人不喜欢使用"xxx等人[引用]提出yyy方法"这种描述,更喜欢"xxx特征的方法去解决yyy问题[引用]"这样的表述,为避免审美疲劳,两种表述方法都可使用,但更要偏向后者

## 写作后
对照[快速检查列表](check_list.md)检查

## 参考文献
http://ws2.nju.edu.cn/kgwiki/doku.php?id=team:writing
