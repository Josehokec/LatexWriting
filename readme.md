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
    - **表示因果**: as a result, because, thus, so, as, since, therefore, consequently, on account of, Ultimately
    - **表示归纳**: as a result, finally, therefore, thus, accordingly, in short, consequently, in conclusion, so, in a word, in brief, certainly, In a nutshell, overall
- 分点让逻辑更清晰
    - Our technique can improve XXX for two reasons. First, xxx. Second, xxx. Third, xxx.
    - We investigate such xxx and discover three reasons. xxx
- 理由要精炼得体,下列语句是摘抄自A类文章,[更多摘抄语句](sentences.txt)
    - Since xx is not open-source, we implement xx from scratch faithfully following the original design principles, as well as caching the top-level nodes on compute nodes for better performance.
    - Since then, both the hardware and workload landscapes have changed.

      
### 公式
- 数学符号: [A short list of commonly used LATEX symbols](https://artofproblemsolving.com/wiki/index.php/LaTeX:Symbols)
- 需编号,**结尾有标点**(下文接where用逗号,没有则用句号),不超宽,等号对齐

### 图表(通常放在论文最顶/底端)
- 算法. 建议使用[algorithm2e package](https://www.ctan.org/pkg/algorithm2e)
- 图片, 见[画图项目](https://github.com/Josehokec/python_figure).
- 表格. 初学者生成表格可以参考[Tables Generator](https://www.tablesgenerator.com)和[Latex-tables](https://www.latex-tables.com)
注意：图标字体统一，字号不大于正文、也不宜过小，标题、图例和坐标轴表达清楚，配色美观

### 引用格式
- 个人不喜欢使用"xxx等人[引用]提出yyy方法"这种描述,更喜欢"xxx特征的方法去解决yyy问题[引用]"这样的表述,有时候避免审美疲劳,两种表述方法都会使用
- 正常来说,去掉引用不应该影响句子的完整性,此外一般我喜欢在引用前加波浪线，如`~\cite{Paper1}`
- 在[dblp](https://dblp.org/)上去寻找获取论文BibTeX,注意:每年论文导入的Bib风格不一样,需要自己修改统一

## 写作后
对照[快速检查列表](check_list.md)检查

## 参考文献
http://ws2.nju.edu.cn/kgwiki/doku.php?id=team:writing
