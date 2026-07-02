# 遗传学100天学习计划 · Day 49

## 遗传力的概念与估算
### Concept and Estimation of Heritability

> **学习日期**: 2026年7月2日 | **Day 49/100** | **第五部分：经典遗传学发展**

---
<!-- Metadata
- Generated: 2026-07-02
- Day: 49
- Topic: 遗传力的概念与估算
- Markdown: https://github.com/lijianguoa/genetics-learning-100-days/blob/main/genetics_day049.md
- Images: https://raw.githubusercontent.com/lijianguoa/genetics-images/main/tree/main/day049
- Notes PPT: https://github.com/lijianguoa/genetics-learning-100-days/blob/main/ppt/genetics_day049_notes.html
- Talk PPT: https://github.com/lijianguoa/genetics-learning-100-days/blob/main/ppt/genetics_day049_talk.html
-->


![遗传力概念图](https://raw.githubusercontent.com/lijianguoa/genetics-images/main/day049/heredity_broad_narrow.jpg)

---

## 一、历史背景

遗传力（Heritability）概念的提出，标志着遗传学从单纯的孟德尔遗传分析迈向了**定量遗传学**（Quantitative Genetics）的新纪元。

### 1.1 从孟德尔到数量遗传学的转折

孟德尔的经典遗传学揭示了质量性状（qualitative traits）——如豌豆的颜色、形状——的遗传规律，这些性状表现为**非此即彼**的离散分布。然而，自然界中大多数经济和生物学上重要的性状——如身高、体重、产奶量、智力等——呈**连续变异**（continuous variation），无法简单用孟德尔定律解释。

19世纪末到20世纪初，统计学家弗朗西斯·高尔顿（Francis Galton）首次系统研究了亲代与子代性状的相关性，提出了**回归分析**（regression analysis）的概念。高尔顿发现，高个子父母的子女平均身高趋向于群体均值——这一现象后来被称为**"向均值回归"（regression toward the mean）**。

### 1.2 Fisher的奠基性贡献

1918年，英国统计遗传学家罗纳德·费舍尔（Ronald A. Fisher）发表了划时代论文 *"The Correlation between Relatives on the Supposition of Mendelian Inheritance"*（[在线阅读](https://doi.org/10.1098/rspb.1918.0012)），首次证明了孟德尔遗传因子可以完美解释连续变异的**生物统计规律**。这篇论文：

- 将孟德尔遗传与生物统计学**统一**为同一框架
- 提出**方差分析**（ANOVA）的基本思想
- 将表型总方差分解为**遗传方差**（genetic variance）和**环境方差**（environmental variance）
- 为现代数量遗传学奠定了数学基础

> Fisher的这篇论文被认为是20世纪最重要的生物学论文之一，"完成了孟德尔革命的最后一块拼图"。—— [Wikipedia: Ronald Fisher](https://en.wikipedia.org/wiki/Ronald_Fisher)

### 1.3 Lush与狭义遗传力

1937年，美国动物育种学家Jay Lush在其经典著作 *"Animal Breeding Plans"* 中首次系统阐述了遗传力的概念，并区分了**广义遗传力**（broad-sense heritability, H²）和**狭义遗传力**（narrow-sense heritability, h²）。Lush的工作将遗传力概念从理论推向了**育种实践**。

---

## 二、核心概念

### 2.1 表型方差的分解

任何数量性状的表型值（P）可以分解为：

$$P = G + E$$

其中：
- **G**（Genotypic value）：基因型值，由遗传因素决定
- **E**（Environmental deviation）：环境偏差，由非遗传因素决定

假设G和E相互独立，则表型方差（Vₚ）等于：

$$V_P = V_G + V_E$$

### 2.2 广义遗传力（Broad-sense Heritability, H²）

$$H^2 = \frac{V_G}{V_P} \times 100\%$$

广义遗传力衡量的是**遗传因素**（包括加性效应、显性效应和上位性效应）占总表型变异的比例。

- **H² = 1**（100%）：表型变异完全由遗传决定
- **H² = 0**（0%）：表型变异完全由环境决定
- 数值范围：0 ≤ H² ≤ 1

### 2.3 狭义遗传力（Narrow-sense Heritability, h²）

$$h^2 = \frac{V_A}{V_P} \times 100\%$$

其中 V_A 为**加性遗传方差**（additive genetic variance）。

狭义遗传力仅考虑**等位基因的加性效应**，是育种实践中最重要的参数：

- 决定了**选择响应**（response to selection）的大小
- 预测亲代与子代之间的**相关性**
- h² 越高，选择效果越好

> **关键区别**：H² 反映遗传因素的总贡献，h² 反映可被选择利用的遗传贡献。在育种中，h² 更具实用价值。—— [Nature Education: Heritability](https://www.nature.com/scitable/topicpage/heritability-518/)

### 2.4 遗传方差的细分

遗传方差 V_G 可以进一步分解：

$$V_G = V_A + V_D + V_I$$

| 成分 | 符号 | 含义 | 能否被选择固定 |
|------|------|------|---------------|
| 加性方差 | V_A | 等位基因累加效应 | 可以 |
| 显性方差 | V_D | 同一基因座等位基因间的互作 | 不能 |
| 上位性方差 | V_I | 不同基因座间的互作效应 | 部分可以 |

---

![遗传力估算方法](https://raw.githubusercontent.com/lijianguoa/genetics-images/main/day049/heritability_estimation.jpg)

---

## 三、科学家故事

### 3.1 罗纳德·费舍尔（Ronald A. Fisher, 1890–1962）

![Ronald Fisher](https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/R._A._Fischer.jpg/220px-R._A._Fischer.jpg)

费舍尔被誉为"现代统计学的奠基人"和"数量遗传学之父"。他的1918年论文在年仅28岁时完成，以一己之力**桥接了孟德尔遗传学派和生物统计学派之间长达十余年的论战**。

费舍尔的贡献远不止遗传力：
- 创立了**最大似然估计**（Maximum Likelihood Estimation）
- 发展了**实验设计**（Design of Experiments）
- 提出了**F检验**和**方差分析**
- 在进化生物学中提出**费舍尔基本定理**（Fisher's Fundamental Theorem of Natural Selection）

> "自然选择的速度等于该时刻的加性遗传方差。" —— Fisher's Fundamental Theorem，[Stanford Encyclopedia of Philosophy](https://plato.stanford.edu/entries/thomas-kuhn/)

### 3.2 杰伊·勒什（Jay L. Lush, 1896–1982）

Lush是美国动物育种学的先驱，在爱荷华州立大学建立了世界上第一个系统的动物育种课程。他首次将遗传力的概念应用于**实际育种方案设计**，极大地提高了奶牛、猪等家畜的育种效率。

### 3.3 西摩·赖特（Sewall Wright, 1889–1988）

 Wright提出了**通径系数分析**（path coefficient analysis）方法，为遗传力估算提供了重要的统计工具。他还独立发展了F统计量（FST），在群体遗传学中具有深远影响。—— [Wikipedia: Sewall Wright](https://en.wikipedia.org/wiki/Sewall_Wright)

---

## 四、重要文献

| 文献 | 作者 | 年份 | 意义 |
|------|------|------|------|
| [*The Correlation between Relatives on the Supposition of Mendelian Inheritance*](https://doi.org/10.1098/rspb.1918.0012) | Fisher, R.A. | 1918 | 数量遗传学奠基之作 |
| [*Animal Breeding Plans*](https://archive.org/details/animalbreedingp00lush) | Lush, J.L. | 1937 | 系统阐述遗传力概念 |
| [*Evolution and the Genetics of Populations*](https://www.press.uchicago.edu/ucp/books/book/chicago/E/bo3638831.html) | Wright, S. | 1968-1978 | 通径分析与遗传方差分解 |
| [*Introduction to Quantitative Genetics*](https://www.amazon.com/Introduction-Quantitative-Genetics-4th/dp/0582243025) | Falconer, D.S. & Mackay, T.F.C. | 1996 | 数量遗传学经典教材（第4版） |
| [*Heritability in the genomics era—concepts and misconceptions*](https://doi.org/10.1038/nrg3806) | Visscher, P.M. et al. | 2017 | 现代遗传力研究的全面综述 |

---

## 五、经典实验

### 5.1 同卵双胞胎 vs. 异卵双胞胎研究

**双胞胎研究**是估算人类复杂性状遗传力的经典方法：

- **同卵双胞胎（MZ）**：遗传物质100%相同
- **异卵双胞胎（DZ）**：平均共享50%的遗传物质

**原理**：如果某一性状的遗传力高，MZ双胞胎的表型相似度应显著高于DZ双胞胎。

**经典案例**：
- **Minnesota双胞胎研究**：对分离抚养的同卵双胞胎进行了长达20年的追踪研究，发现智商（IQ）的遗传力约为0.70—— [Minnesota Twin Family Study](https://mtfs.umn.edu/)
- **明尼苏达双胞胎登记处**数据表明：身高的遗传力约为0.80，体重指数（BMI）约为0.50-0.70

### 5.2 亲子回归分析

通过测量亲代与子代性状值，利用**回归斜率**估算遗传力：

$$b_{OP} = \frac{1}{2}h^2$$

其中 b_OP 为子代对中亲值的回归系数。

**Falconer公式**：
- 子代-中亲回归：h² = 2 × b_OP
- 半同胞分析：h² = 4 × r_HS（半同胞相关系数）
- 全同胞分析：需校正显性效应

### 5.3 选择实验

**选择实验**直接验证遗传力的预测能力：

$$R = h^2 \times S$$

其中：
- **R**（Response）：选择响应（子代均值相对于群体均值的变化）
- **S**（Selection differential）：选择差（被选亲本均值与群体均值之差）
- **h²**：狭义遗传力

**经典案例**：芝加哥大学的**Long-Term Selection Experiment on Corn**（伊利诺伊大学玉米蛋白质和含油量选择实验，1896年持续至今），已经进行了超过100代的选择，充分验证了遗传力在预测选择响应中的核心作用。—— [University of Illinois: Selection Experiment](https://agronomy.illinois.edu/illinois-long-term-selection-experiment)

---

## 六、小故事

### "丢失的遗传力"问题（Missing Heritability Problem）

2000年代初，随着全基因组关联分析（GWAS）技术的发展，遗传学家兴奋地发现可以定位大量与复杂性状相关的遗传变异。然而，一个令人困惑的现象出现了：GWAS发现的所有SNP共同解释的表型变异比例**远低于**传统双胞胎研究估算的遗传力。

例如：
- 人类身高的遗传力约80%，但2008年首批GWAS仅找到约5%的解释量
- 这被称为**"丢失的遗传力"**（Missing Heritability）

**解决方案**逐渐浮出水面：
1. **罕见变异**（rare variants）：GWAS主要检测常见变异（MAF > 5%），但罕见变异也贡献遗传力
2. **高度多效性**（polygenicity）：身高等性状由数千甚至数万个位点共同控制，每个效应极小
3. **遗传相关性**（linkage disequilibrium）：邻近变异间的相关性影响独立效应的估计
4. **基因-环境互作**和**表观遗传效应**—— [Nature: Missing Heritability](https://www.nature.com/articles/nrg2761)

2010年代的研究表明，当使用**全基因组复杂性状分析**（GREML/Genomic SEM）等方法时，常见SNP可以解释大部分遗传力——"丢失"的遗传力并未真正丢失，只是分散在大量效应极小的变异中。

---

## 七、思考题

1. **基础题**：如果某一性状的广义遗传力H² = 0.6，狭义遗传力h² = 0.3，请解释V_D和V_I相对于V_A的大小关系。

2. **应用题**：在一个奶牛群体中，产奶量的选择差S = 2000 kg，狭义遗传力h² = 0.25，预计下一代的选择响应R是多少？如果连续选择5代，累计响应是多少？

3. **思辨题**：遗传力是否等同于"遗传决定度"？为什么"遗传力高"不意味着"环境不重要"？请结合**群体内遗传力**和**群体间遗传力**的区别来讨论。

4. **拓展题**：什么是"丢失的遗传力"问题？当前的解决方案有哪些？请查阅近5年的文献，了解GWAS和全基因组遗传力估算（GREML/LDSC）的最新进展。

---

## 八、术语表

| 英文术语 | 缩写 | 中文翻译 | 简要说明 |
|----------|------|----------|----------|
| Heritability (broad-sense) | H² | 广义遗传力 | 遗传方差占总表型方差的比例 |
| Heritability (narrow-sense) | h² | 狭义遗传力 | 加性遗传方差占总表型方差的比例 |
| Phenotypic variance | Vₚ | 表型方差 | 群体中某性状表型值的变异程度 |
| Genotypic variance | V_G | 遗传方差 | 由遗传因素引起的方差 |
| Additive genetic variance | V_A | 加性遗传方差 | 等位基因累加效应引起的方差 |
| Dominance variance | V_D | 显性方差 | 同一基因座等位基因互作效应的方差 |
| Epistatic variance | V_I | 上位性方差 | 不同基因座间互作效应的方差 |
| Environmental variance | V_E | 环境方差 | 由非遗传因素引起的方差 |
| Selection differential | S | 选择差 | 被选亲本均值与群体均值之差 |
| Response to selection | R | 选择响应 | 子代均值相对于群体均值的变化 |
| Breeder's equation | — | 育种者方程 | R = h² × S |
| Regression toward the mean | — | 向均值回归 | 极端值亲代的子代趋向群体均值 |
| Missing heritability | — | 丢失的遗传力 | GWAS未解释的遗传力部分 |
| GREML | — | 全基因组限制性最大似然 | 利用全基因组SNP估算遗传力的方法 |
| GWAS | — | 全基因组关联分析 | 检测性状与基因组变异关联的方法 |

---

## 九、下节预告

**Day 50：群体遗传学的诞生**

明天我们将进入群体遗传学的世界！从个体水平的遗传分析跃升到**群体水平**，探讨基因频率在群体中的变化规律。我们将学习：

- 哈代-温伯格定律（Hardy-Weinberg Equilibrium）——群体遗传学的"零模型"
- 等位基因频率与基因型频率的数学关系
- 遗传漂变、突变、迁移、选择如何改变群体遗传结构

这是理解**进化遗传学**的基础，也是现代基因组学数据分析的核心理论框架。敬请期待！

---

> **📚 推荐资源**
> - [Wikipedia: Heritability](https://en.wikipedia.org/wiki/Heritability) — 遗传力百科全书条目
> - [Nature Scitable: Heritability](https://www.nature.com/scitable/topicpage/heritability-518/) — 可视化教学
> - [YouTube: Heritability Explained](https://www.youtube.com/results?search_query=heritability+explained+genetics) — 视频教程
> - [B站：遗传力与数量遗传学](https://search.bilibili.com/all?keyword=遗传力+数量遗传学) — 中文视频资源
> - [NCBI: Quantitative Trait Locus](https://www.ncbi.nlm.nih.gov/genome/qtl/) — NCBI数量性状基因座数据库
> - [Falconer & Mackay: Introduction to Quantitative Genetics](https://www.amazon.com/Introduction-Quantitative-Genetics-4th/dp/0582243025) — 经典教材

---

*遗传学100天学习计划 · Day 49 · 2026年7月2日*

> **🔗 扩展学习资源（自动收录）**
> - [Khan Academy: Heritability](https://www.khanacademy.org/science/ap-biology/natural-selection/heritability-and-variation/a/heritability) — 可汗学院遗传力教程
> - [YouTube: Quantitative Genetics - Heritability](https://www.youtube.com/results?search_query=quantitative+genetics+heritability+lecture) — 精选视频课程
> - [B站: 数量遗传学基础](https://search.bilibili.com/all?keyword=数量遗传学+遗传力) — 中文字幕课程
> - [NCBI Bookshelf: Quantitative Genetics](https://www.ncbi.nlm.nih.gov/books/NBK21356/) — NCBI在线教材
> - [Wikipedia: Quantitative Genetics](https://en.wikipedia.org/wiki/Quantitative_genetics) — 数量遗传学百科
> - [PLoS: Estimating Heritability](https://journals.plos.org/plosgenetics/article?id=10.1371/journal.pgen.1004453) — 遗传力估算方法综述
*自动生成于 genetics-learning-100-days 项目*
