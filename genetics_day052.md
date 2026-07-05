# Day 52 | 基因频率与进化

> **遗传学100天学习计划** · 第五部分：经典遗传学发展（Day 46-60）
> **日期**：2026年7月5日
> **系列进度**：52/100

---

## 配图 Illustrations

| 图片 | 描述 |
|------|------|
| ![基因频率变化示意图](day052_gene_frequency_evolution.png) | 基因频率在自然选择作用下的世代变化趋势 |
| ![进化动力全景图](day052_evolution_forces_panorama.png) | 驱动基因频率变化的四大进化动力全景 |

---

## 历史背景 Historical Background

基因频率（Gene Frequency）与进化的定量研究是20世纪初群体遗传学诞生的直接产物。在孟德尔定律于1900年被重新发现之后，遗传学家面临一个核心问题：**孟德尔遗传定律如何与达尔文的自然选择理论相统一？**

1908年，英国数学家哈迪（G.H. Hardy）和德国医生温伯格（Wilhelm Weinberg）各自独立提出了**哈迪-温伯格平衡定律**（Hardy-Weinberg Equilibrium），证明了在没有进化力量作用时，一个随机交配群体中的基因频率和基因型频率在世代间保持恒定。这一定律为衡量进化是否发生提供了**零假设（null hypothesis）**。

然而，真正将基因频率变化与进化机制建立定量联系的，是**R.A. Fisher**、**J.B.S. Haldane**和**Sewall Wright**三位群体遗传学奠基人：

- **Fisher**（1918年）在论文《The Correlation between Relatives on the Supposition of Mendelian Inheritance》中证明，连续变异可以用大量孟德尔基因的累加效应来解释，从而**统一了孟德尔遗传与生物统计学派**。
- **Haldane**（1924-1932年）系统计算了自然选择的强度、突变压力和迁移对基因频率变化的影响，提出了**选择系数（selection coefficient）** 的概念。
- **Wright**（1931年）引入了**有效群体大小（effective population size, Ne）**、**遗传漂变（genetic drift）** 和**适应度景观（adaptive landscape）** 等核心概念。

这三位科学家的工作共同构成了**现代进化综合论（Modern Synthesis）** 的数学基础，将遗传学、进化论和分类学融为一体。

---

## 核心概念 Core Concepts

### 1. 基因频率（Gene Frequency / Allele Frequency）

基因频率是指在一个群体中，某一位点上特定等位基因占全部等位基因的比例。

$$p = \frac{\text{某等位基因的拷贝数}}{\text{该位点所有等位基因的总拷贝数}}$$

**示例**：在一个二倍体群体中，基因座A有两个等位基因 A 和 a：
- 基因型 AA = 36个个体，Aa = 48个个体，aa = 16个个体
- 总个体数 N = 100，总等位基因数 = 2N = 200
- A 的频率：p = (2×36 + 48) / 200 = 120/200 = **0.6**
- a 的频率：q = (2×16 + 48) / 200 = 80/200 = **0.4**
- p + q = 1.0

> 📖 **延伸阅读**：[Allele Frequency - NCBI](https://www.ncbi.nlm.nih.gov/books/NBK21976/) | [基因频率 - Wikipedia](https://zh.wikipedia.org/wiki/基因频率)

### 2. 基因型频率（Genotype Frequency）

基因型频率是群体中某种基因型个体占总个体数的比例。在哈迪-温伯格平衡下：

$$P(AA) = p^2, \quad P(Aa) = 2pq, \quad P(aa) = q^2$$

### 3. 进化的遗传学定义

在现代群体遗传学中，**进化被定义为群体中基因频率随时间的变化**。当 p(A) 在世代间发生变化时，进化就在发生。影响基因频率变化的力量有四种：

| 进化力量 | 作用机制 | 速度 |
|----------|----------|------|
| **自然选择** | 差异化生存与繁殖 | 可快可慢 |
| **遗传漂变** | 随机抽样效应 | 小群体中显著 |
| **基因流/迁移** | 群体间个体迁移 | 取决于迁移率 |
| **突变** | 等位基因的随机改变 | 通常非常缓慢 |

### 4. 适合度（Fitness, W）

适合度衡量某基因型个体将其等位基因传递给下一代的能力：

$$W = 1 - s$$

其中 s 为**选择系数（selection coefficient）**，表示选择对该基因型不利作用的强度。

### 5. 选择对基因频率变化的影响

**正向选择（Positive Selection）**：有利等位基因频率逐渐增加

$$\Delta p \approx \frac{spq^2}{1 - sq^2}$$

**负向选择（Purifying Selection）**：有害等位基因频率逐渐降低

**平衡选择（Balancing Selection）**：维持多态性，包括：
- **杂合子优势（Heterozygote Advantage）**：如镰刀形细胞贫血症与疟疾抗性
- **频率依赖选择（Frequency-dependent Selection）**

> 📖 **延伸阅读**：[Natural Selection - Wikipedia](https://en.wikipedia.org/wiki/Natural_selection) | [群体遗传学 - Wikipedia](https://zh.wikipedia.org/wiki/群体遗传学)

---

## 科学家故事 Scientist Story

### R.A. Fisher —— 用数学统一遗传与进化

**罗纳德·艾尔默·费舍尔**（Sir Ronald Aylmer Fisher, 1890-1962）是20世纪最伟大的统计学家和进化生物学家之一。

Fisher出生于英国伦敦，从小展现出非凡的数学天赋。他在剑桥大学学习数学和物理学期间，受到孟德尔遗传学重新发现的启发，开始思考如何将数学方法应用于遗传学问题。

**关键贡献**：

1. **1918年论文**：Fisher在《Mendelian Inheritance》这篇划时代论文中，证明了连续变异（如身高、体重）可以用大量孟德尔因子的累加效应来解释。这篇论文终结了"孟德尔学派"与"生物统计学派"长达十余年的争论。

2. **《The Genetical Theory of Natural Selection》（1930年）**：这是群体遗传学的奠基之作。Fisher在书中提出了**基本定理（Fisher's Fundamental Theorem of Natural Selection）**：

   > *"任何时刻，适合度的增加率等于适合度的遗传方差。"*
   > （The rate of increase in fitness of any organism at any time is equal to its genetic variance in fitness at that time.）

3. **方差分析（ANOVA）**：Fisher发明了这一至今仍是统计学核心工具的方法。

Fisher性格刚烈，与许多同行关系紧张，特别是与Haldane和Wright之间的学术分歧持续了数十年。但正是这三位科学家的竞争与合作，推动了现代进化综合论的诞生。

> 📖 **延伸阅读**：[R.A. Fisher - Wikipedia](https://en.wikipedia.org/wiki/Ronald_Fisher) | [Fisher's Fundamental Theorem](https://en.wikipedia.org/wiki/Fisher%27s_fundamental_theorem)

---

## 重要文献 Key Literature

| 文献 | 作者 | 年份 | 核心贡献 |
|------|------|------|----------|
| [Mendel's Laws of Heredity](https://www.esp.org/sites/classics/library/fisher/1936.pdf) | Fisher | 1918 | 证明连续变异的孟德尔基础 |
| [A Mathematical Theory of Natural and Artificial Selection](https://doi.org/10.1017/S0013091500011976) | Haldane | 1924-1932 | 系统推导选择对基因频率的影响 |
| [Evolution in Mendelian Populations](https://www.pnas.org/doi/10.1073/pnas.17.2.109) | Wright | 1931 | 引入漂变、有效群体大小 |
| [The Genetical Theory of Natural Selection](https://archive.org/details/geneticaltheor00fish) | Fisher | 1930 | 群体遗传学奠基之作 |
| [The Causes of Evolution](https://archive.org/details/causesofevoluti00hald) | Haldane | 1932 | 自然选择的代价——Haldane困境 |
| [Genetics and the Origin of Species](https://archive.org/details/geneticsandorig00dobz) | Dobzhansky | 1937 | 现代进化综合论的经典表述 |

> 📖 **延伸阅读**：[Modern Evolutionary Synthesis - Wikipedia](https://en.wikipedia.org/wiki/Modern_synthesis_(20th_century))

---

## 经典实验 Classic Experiments

### 实验1：工业黑化（Industrial Melanism）——桦尺蠖的自然选择

**背景**：19世纪的工业革命使英国中北部地区大量树木被煤烟熏黑。1850年代，桦尺蠖（*Biston betularia*）种群中黑色型（carbonaria）的频率急剧上升。

**关键证据**：
- **Kettlewell（1955年）**的标记-重捕实验：
  - 在被煤烟污染的伯明翰地区，黑色型存活率远高于浅色型（typica）
  - 在未污染的多塞特地区，浅色型存活率远高于黑色型
  - 数据证实了**定向自然选择**正在改变基因频率

**基因频率变化记录**：
- 1848年：黑色型突变等位基因频率接近 0
- 1895年：曼彻斯特地区黑色型频率达到约 **98%**
- 1960年代后：随着空气污染治理，浅色型频率开始回升

这一案例完美展示了自然选择如何改变基因频率，是进化生物学教科书中的经典案例。

> 📖 **延伸阅读**：[Industrial Melanism - Wikipedia](https://en.wikipedia.org/wiki/Industrial_melanism_in_the_peppered_moth) | [Biston betularia - NCBI](https://www.ncbi.nlm.nih.gov/Taxonomy/Browser/wwwtax.cgi?id=73914)

### 实验2：DDT抗性实验

**过程**：对果蝇群体施用DDT杀虫剂：
1. 初始群体中几乎不存在抗性等位基因
2. 绝大多数个体死亡，极少数携带隐性抗性基因的个体存活
3. 存活个体交配后，抗性等位基因频率急剧上升
4. 经过数代选择后，整个群体产生高度抗性

**结论**：强大的定向选择可以在短短数代内将极低频率的有利等位基因提升到高频率——这被称为**"选择的快车道"**。

> 📖 **延伸阅读**：[Pesticide Resistance - NCBI](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3230959/)

---

## 小故事 Anecdote

### "费舍尔的对数"与基本定理

Fisher在构思他的基本定理时，据说有一次在剑桥的花园中散步，突然意识到**适合度的对数（log fitness）可以线性分解为基因的平均效应之和**。他激动地跑回办公室，在一张餐巾纸上写下了关键公式。

这一洞察的核心在于：虽然适合度本身是非线性的（因为它涉及基因型间的相互作用），但**在对数尺度上，每个基因位点对适合度的贡献是近似独立的**。这使得自然选择可以同时作用于多个位点，而不必考虑它们之间的复杂相互作用。

这个看似简单的数学性质，为理解多基因同时进化提供了坚实的理论基础，也解释了为什么自然界中的进化通常是渐进的，而非跳跃式的。

> 后来Haldane评价这一发现时说："Fisher的基本定理就像是牛顿第二定律对进化生物学的意义。"

---

## 思考题 Discussion Questions

1. **计算题**：在一个1000人的群体中，MN血型基因座的基因型分布为：MM=200人，MN=500人，NN=300人。请计算M和N等位基因的频率，并检验是否符合哈迪-温伯格平衡。

2. **思考题**：如果一个小岛上的昆虫种群只有50个个体，而大陆上的同种昆虫有10万个个体，遗传漂变对这两个群体基因频率的影响有何不同？

3. **辨析题**：自然选择能否创造新的等位基因？如果不能，新的遗传变异是从哪里来的？

4. **讨论题**：Haldane困境（the cost of natural selection）指出，当多个基因座同时受到选择时，所需的替代时间可能超过物种存活时间。这一理论困难如何被现代遗传学解决？

5. **应用题**：在人类群体中，导致镰刀形细胞贫血症的HbS等位基因在某些疟疾流行地区的频率可高达15%。请用杂合子优势（heterozygote advantage）解释这一现象，并计算各基因型的频率。

> 📖 **延伸阅读**：[Haldane's Dilemma - Wikipedia](https://en.wikipedia.org/wiki/Haldane%27s_dilemma) | [Sickle Cell and Malaria - NCBI](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3076740/)

---

## 术语表 Glossary

| 术语 | 英文 | 定义 |
|------|------|------|
| 基因频率 | Gene / Allele Frequency | 特定等位基因占该位点全部等位基因的比例 |
| 基因型频率 | Genotype Frequency | 某种基因型个体占总个体数的比例 |
| 适合度 | Fitness (W) | 个体或基因型将基因传递给后代的能力 |
| 选择系数 | Selection Coefficient (s) | 1 - W，衡量选择压力的强度 |
| 有效群体大小 | Effective Population Size (Ne) | 对遗传漂变影响等价的理想群体个体数 |
| 遗传漂变 | Genetic Drift | 由于随机抽样导致的基因频率变化 |
| 基因流 | Gene Flow / Migration | 群体间个体迁移引起的基因频率变化 |
| 固定 | Fixation | 某一等位基因频率变为1（纯合） |
| 丢失 | Loss | 某一等位基因频率变为0 |
| 多态性 | Polymorphism | 同一基因座存在多个等位基因 |
| 杂合子优势 | Heterozygote Advantage | 杂合子适合度高于两种纯合子的现象 |
| Fisher基本定理 | Fisher's Fundamental Theorem | 适合度的变化率等于其遗传方差 |
| 现代进化综合论 | Modern Synthesis | 综合遗传学与进化论的综合性框架 |
| 连锁不平衡 | Linkage Disequilibrium | 不同基因座等位基因的非随机关联 |

> 📖 **延伸阅读**：[Population Genetics Glossary - Nature](https://www.nature.com/subjects/population-genetics)

---

## 下节预告 Next Day Preview

### Day 53 | 自然选择与遗传

明天我们将深入探讨**自然选择（Natural Selection）** 如何在遗传学层面上发挥作用。主要内容包括：

- **选择的不同模式**：定向选择（directional selection）、稳定选择（stabilizing selection）、分裂选择（disruptive selection）
- **选择的单位之争**：基因选择 vs. 个体选择 vs. 群体选择
- **Haldane的选择代价理论**
- **分子层面的自然选择证据**：dN/dS比值分析
- **人工选择与自然选择的比较**

> **预习建议**：复习Day 51哈迪-温伯格定律的推导过程，并提前阅读Haldane 1924年的经典论文 [A Mathematical Theory of Natural and Artificial Selection](https://doi.org/10.1017/S0013091500011976)。

---

## 学习资源汇总 Learning Resources

### 视频资源
- [基因频率与进化 - YouTube (Khan Academy)](https://www.youtube.com/watch?v=4KborikITB0)
- [群体遗传学入门 - B站](https://www.bilibili.com/video/BV1mb411q7qZ)
- [Hardy-Weinberg Equilibrium Explained - YouTube](https://www.youtube.com/watch?v=9F5Oz8AoNkQ)

### 文献资源
- [Population Genetics - NCBI Bookshelf](https://www.ncbi.nlm.nih.gov/books/NBK21972/)
- [Genetic Variation - NCBI](https://www.ncbi.nlm.nih.gov/books/NBK21580/)
- [The Modern Synthesis - Stanford Encyclopedia of Philosophy](https://plato.stanford.edu/entries/biology-synthesis/)

---

*📅 本期内容发布于2026年7月5日 | 遗传学100天学习计划 Day 52/100*
*🔔 欢迎关注 [GitHub仓库](https://github.com/lijianguoa/genetics-learning-100-days) 获取每日更新*
