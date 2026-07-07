# 遗传学100天学习计划 · Day 54

## 🧬 遗传漂变（Genetic Drift）

> **学习日期**：2026年7月7日（Day 54）
> **所属模块**：第五部分 · 经典遗传学发展（Day 46–60）
> **前一日**：[Day 53 · 自然选择与遗传](https://github.com/lijianguoa/genetics-learning-100-days/blob/main/genetics_day053.md)
> **后一日**：[Day 55 · 迁移与基因流](https://github.com/lijianguoa/genetics-learning-100-days/blob/main/genetics_day055.md)

---

## 📸 配图

| 图片 | 说明 |
|------|------|
| ![遗传漂变示意图](genetics_day054_drift_diagram.png) | **遗传漂变模拟示意图**：展示等位基因频率在世代间的随机变化，最终走向固定或丢失 |
| ![创始者效应与瓶颈效应](genetics_day054_founder_bottleneck.png) | **创始者效应与瓶颈效应对比图**：展示两种漂变的典型场景及其对遗传多样性的影响 |

---

## 📜 历史背景

### 漂变概念的孕育

遗传漂变（Genetic Drift）的思想起源可以追溯到更早的时期。达尔文在《物种起源》（1859）中曾提及"中性变异"可能最终固定，但并未对此做深入探讨。

- **1873年**：美国传教士兼博物学家 **John Gulick** 在研究夏威夷群岛相似环境中蜗牛形态的巨大差异时，率先提出小种群中变异可通过随机过程保留，这一观察被认为是漂变概念的萌芽。
- **1921年**：荷兰遗传学家 **Hagedoorn & Hagedoorn** 首次系统描述了"随机采样"导致变异减少的现象，指出小群体比大群体更快趋向纯合（固定）。

### "漂变"术语的诞生

- **1929年**：**Sewall Wright** 首次使用"drift"一词描述随机遗传变化。
- **1931年**：Wright 发表里程碑论文 *"Evolution in Mendelian Populations"*（发表于 *Genetics* 16: 97–159），**正式而清晰**地描述了遗传漂变的过程——在有限种群中，配子的随机采样导致等位基因频率的随机变化。

### 20世纪中叶的争论

Wright 与 **R.A. Fisher** 围绕漂变在进化中的重要性展开了著名的学术论争。Fisher 认为在大种群中漂变效应太弱，进化主要由自然选择驱动；而 Wright 认为即使是中等大小的种群，漂变也能发挥重要进化作用。

**1968年**，**木村资生（Motoo Kimura）** 发表 *"Evolutionary Rate at the Molecular Level"*（*Nature* 217: 624–626），提出了**分子进化中性理论**，将漂变的地位提升到分子进化的核心驱动力，引发了持续数十年的中性论与选择论之争。

> 📖 **延伸阅读**：
> - Wright (1931) 论文原文：[JSTOR](https://www.jstor.org/stable/2448780)
> - Kimura (1968) Nature 论文：[Nature](https://www.nature.com/articles/217624a0)
> - 斯坦福哲学百科 · Genetic Drift：[Stanford Encyclopedia of Philosophy](https://plato.stanford.edu/entries/genetic-drift/)

---

## 🔬 核心概念

### 1. 遗传漂变的定义

遗传漂变是指在有限种群中，由于**随机抽样误差（sampling error）**导致的等位基因频率的**随机变化**。这种变化不是由自然选择驱动的，而是由随机生育、死亡和孟德尔分离等随机过程产生。**种群越小，漂变效应越强**。

### 2. 创始者效应（Founder Effect）

当少数个体从大种群中分离出去建立新种群时，新种群的等位基因频率可能与源种群**显著不同**。

**特征**：
- 新种群遗传多样性大幅降低
- 某些等位基因频率异常升高或降低
- 罕见等位基因可能在新种群中变得常见

**经典案例**：
- **宾夕法尼亚州阿米什人（Amish）**：约200名创始人建立种群，Ellis-van Creveld综合征（多指畸形、矮小等）发病率远高于普通人群（约1/200 vs 1/60,000）
- **冰岛人群**：约800–1000名维京定居者奠基，形成了独特的遗传病谱系

> 📖 [Khan Academy · Founder Effect 详解](https://en.khanacademy.org/science/biology/her/heredity-and-genetics/a/genetic-drift-founder-bottleneck)

### 3. 瓶颈效应（Population Bottleneck）

种群因灾难（疾病、捕杀、自然灾害等）急剧缩减，幸存者的基因库丧失大部分遗传多样性。

**经典案例**：

| 案例 | 描述 | 现状 |
|------|------|------|
| **北象海豹** | 19世纪末被捕杀至约20只 | 虽恢复至数十万只，但遗传多样性极低 |
| **猎豹** | 经历严重瓶颈效应 | 种内遗传多样性极低，个体间可互相皮肤移植 |
| **平塔岛象龟"孤独乔治"** | 种群锐减至单一个体 | 该亚种于2012年宣告灭绝 |

### 4. 有效种群大小（Effective Population Size, Ne）

Wright 的定义：**"在随机漂变或近交方面表现出与实际群体相同等位基因频率分散程度的理想群体中的繁殖个体数。"**

通常 **Ne 远小于实际种群数量 N**，原因包括：
- 性别比不等（如一夫多妻制）
- 繁殖成功率差异
- 种群大小波动

**核心公式**：每代杂合度损失率 = **1/(2Ne)**

等位基因频率变化的方差：**Var(Δp) = p(1-p) / (2Ne)**

### 5. 固定与丢失（Fixation & Loss）

- **固定**：某等位基因在种群中频率达到100%
- **丢失**：某等位基因在种群中频率降为0%

**中性等位基因的固定概率**：**P = 1/(2N)**（N为有效种群大小）

**木村资生公式（1962）**：对于具有选择优势 s 的等位基因：
**P = (1 - e^(-2s)) / (1 - e^(-4Ns))**

### 6. 遗传漂变 vs 自然选择

| 特征 | 遗传漂变 | 自然选择 |
|------|----------|----------|
| 驱动力 | 随机抽样误差 | 环境筛选压力 |
| 方向 | 随机（无方向性） | 定向（适应环境） |
| 种群大小效应 | 小种群效应强 | 任何大小种群都有效 |
| 结果 | 固定或丢失（随机） | 适应性等位基因频率增加 |
| 速度 | 与 1/(2Ne) 成正比 | 与选择系数 s 成正比 |

---

## 👨‍🔬 科学家故事

### Sewall Wright（1889–1988）—— 遗传漂变之父

![Sewall Wright](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5f/Sewall_Wright.jpg/220px-Sewall_Wright.jpg)

Sewall Wright 是美国群体遗传学家，遗传漂变理论的主要创立者，与 R.A. Fisher 和 J.B.S. Haldane 并列为**群体遗传学三大奠基人**。

**主要贡献**：
- 发明了**近交系数（Inbreeding Coefficient, F）**和**F统计量（Fst, Fit, Fis）**，成为群体遗传学的标准工具
- 提出了**转移平衡理论（Shifting Balance Theory, 1932）**，描述遗传漂变与选择、迁移相互作用的适应性进化过程
- 1929年首次使用"drift"一词，1931年发表经典论文系统描述漂变

Wright 是一位多产的学者，其数学天赋使群体遗传学从定性描述走向定量分析。他的 F统计量至今仍是衡量种群分化和近交程度的核心指标。

> 📖 [Wikipedia · Sewall Wright](https://en.wikipedia.org/wiki/Sewall_Wright)

### 木村资生（Motoo Kimura, 1924–1994）—— 中性理论之父

![Motoo Kimura](https://upload.wikimedia.org/wikipedia/commons/thumb/2/23/Motoo_Kimura.jpg/220px-Motoo_Kimura.jpg)

木村资生是日本群体遗传学家，**分子进化中性理论**的创立者。1968年在 *Nature* 发表短文提出中性理论，主张**大多数分子水平的遗传变异（氨基酸替换、碱基替换）是中性的**，其频率变化主要由随机漂变驱动。

**核心洞察**：哺乳动物基因组中核苷酸替换的总速率远超 Haldane（1957）提出的"自然选择代价"上限，因此大量分子替换必然是中性的。

**学术争论**：中性理论引发了持续数十年的"中性论 vs 选择论"大辩论。木村资生在1983年出版的 *The Neutral Theory of Molecular Evolution* 中对理论进行了系统阐述。尽管其理论的某些方面后来被修正（如太田朋子的"近乎中性理论"），但漂变作为分子进化的核心驱动力已得到广泛认可。

> 📖 [Wikipedia · Motoo Kimura](https://en.wikipedia.org/wiki/Motoo_Kimura)

---

## 📚 重要文献

| # | 文献 | 期刊/出处 | 年份 | 核心贡献 |
|---|------|-----------|------|----------|
| 1 | Wright, S. *"Evolution in Mendelian Populations"* | Genetics 16: 97–159 | 1931 | 遗传漂变理论的奠基之作 |
| 2 | Wright, S. *"The Roles of Mutation, Inbreeding, Crossbreeding, and Selection in Evolution"* | Proc. 6th Int. Cong. Genetics | 1932 | 转移平衡理论的首次阐述 |
| 3 | Buri, P. *"Gene Frequency in Small Populations of Mutant Drosophila"* | Evolution 10: 367–402 | 1956 | 实验验证遗传漂变的经典论文 |
| 4 | Haldane, J.B.S. *"The Cost of Natural Selection"* | Journal of Genetics 55: 511–524 | 1957 | 自然选择代价，间接支持中性理论 |
| 5 | Kimura, M. *"On the Probability of Fixation of Mutant Genes in a Population"* | Genetics 47: 713–719 | 1962 | 固定概率公式 |
| 6 | Kimura, M. *"Evolutionary Rate at the Molecular Level"* | Nature 217: 624–626 | 1968 | **中性理论的奠基论文** |
| 7 | Kimura, M. & Ohta, T. *Theoretical Aspects of Population Genetics* | Princeton University Press | 1971 | 中性理论的系统论述 |
| 8 | Ohta, T. *"Slightly deleterious mutant substitutions in evolution"* | Nature 246: 96–98 | 1973 | "近乎中性理论"的提出 |

> 📖 **在线阅读**：
> - Kimura (1968) Nature 原文：[Nature](https://www.nature.com/articles/217624a0)
> - NCBI Bookshelf · Population Genetics：[Gene in Populations](https://www.ncbi.nlm.nih.gov/books/NBK21122/)
> - 木村资生中性理论25周年回顾（PMC）：[PMC1203127](https://pmc.ncbi.nlm.nih.gov/articles/PMC1203127/pdf/183.pdf)

---

## 🧪 经典实验

### Buri 的果蝇眼色实验（1956）—— 最经典的遗传漂变实验

**实验者**：Peter Buri（Sewall Wright 的学生）

**实验设计**：
- 建立了 **107个果蝇（Drosophila melanogaster）实验种群**
- 每个种群 8雄8雌（共16只）
- 全部为 *bw*（褐色眼）和 *bw^75*（亮褐眼）等位基因的**杂合子**
- 初始等位基因频率各为 **0.5**
- 连续繁殖 **19代**

**实验结果**：
1. 107个种群中等位基因频率呈现**广泛的随机分散**
2. 随着世代推进，频率分布从集中在0.5逐渐向两端扩散
3. 到第19代，种群逐渐向 *bw* 或 *bw^75* 的**固定（fixation）**收敛
4. 最终几乎所有种群都固定为其中一种等位基因

**实验意义**：
- **首次以实验方式**直观展示了遗传漂变导致等位基因频率随机变化和最终固定的全过程
- 结果与 **Wright-Fisher 模型**的理论预测高度吻合
- 证明了即使是中性等位基因，在小种群中也会因随机抽样而固定或丢失

> 📖 Buri (1956) 原文：[JSTOR](https://www.jstor.org/stable/2406602)
> 📹 **视频资源**：
> - [JoVE · Genetic Drift（中文字幕）](https://www.jove.com/cn/science-education/v/11128/genetic-drift)

---

## 📖 小故事

### 北象海豹的"过山车"命运

北象海豹（*Mirounga angustirostris*）的故事是瓶颈效应最经典的案例之一。

19世纪，由于大规模的商业捕杀，北象海豹种群从数十万只锐减至**仅剩约20只**。这种极端的瓶颈效应导致了极其严重的后果：即使后来种群恢复到了数十万只，但其**遗传多样性仍然极低**。

科学家对北象海豹的基因检测显示，它们的线粒体DNA变异几乎为零，与南象海豹相比，遗传多样性低了一个数量级。这意味着如果未来面临新的疾病威胁或环境变化，北象海豹可能因缺乏遗传适应能力而再次陷入危机。

这个故事告诉我们：**种群数量可以恢复，但遗传多样性一旦丧失，几乎不可逆转。**

### "孤独乔治"—— 最后一个

2012年6月24日，平塔岛象龟（*Chelonoidis abingdoni*）"孤独乔治"（Lonesome George）在加拉帕戈斯群岛去世。它是其物种的**最后一个已知个体**。

孤独乔治的命运是遗传漂变和种群瓶颈的极端案例——种群逐渐缩小，最终因漂变和近交效应丧失了维持种群所需的遗传多样性。它的离世标志着一个亚种的**永久消失**，也成为了物种保护运动的重要象征。

> 📖 [Wikipedia · Lonesome George](https://en.wikipedia.org/wiki/Lonesome_George)

---

## 🤔 思考题

1. **基础题**：在一个有效种群大小 Ne=50 的群体中，一个新产生的中性突变最终被固定的概率是多少？如果一个新突变是致死的呢？

2. **理解题**：比较创始者效应和瓶颈效应的异同点。为什么两者都会导致遗传多样性降低，但其机制不同？

3. **分析题**：假设有一个种群经历了瓶颈效应后种群数量恢复，为什么该种群的进化潜力可能反而比瓶颈前更低？

4. **思辨题**：如果遗传漂变是随机的，为什么它在进化中仍然重要？请结合中性理论说明漂变与自然选择的关系。

5. **应用题**：在进行濒危物种保护时，如何考虑遗传漂变的影响？最小存活种群（MVP）的确定与有效种群大小有何关系？

---

## 📝 术语表

| 术语 | 英文 | 定义 |
|------|------|------|
| **遗传漂变** | Genetic Drift | 因随机抽样误差导致的群体等位基因频率变化 |
| **创始者效应** | Founder Effect | 少数个体建立新种群，新种群基因频率与源种群显著不同 |
| **瓶颈效应** | Population Bottleneck | 种群急剧缩减后遗传多样性大幅丧失 |
| **有效种群大小** | Effective Population Size (Ne) | 理想Wright-Fisher群体中产生相同漂变速率的繁殖个体数 |
| **固定** | Fixation | 某一等位基因在种群中频率达到100% |
| **丢失** | Loss | 某一等位基因在种群中频率降为0% |
| **固定概率** | Fixation Probability | 新突变最终在种群中固定的概率 |
| **近交系数** | Inbreeding Coefficient (F) | 个体在某个基因座上两个等位基因来自共同祖先的概率 |
| **F统计量** | F-statistics (Fst, Fit, Fis) | 衡量种群分层和近交程度的统计量 |
| **转移平衡理论** | Shifting Balance Theory | Wright提出的漂变与选择相互作用的适应性理论 |
| **中性理论** | Neutral Theory | 木村资生提出，主张大多数分子变异由漂变驱动 |
| **近乎中性理论** | Nearly Neutral Theory | Ohta（1973）提出，弱有害突变在小种群中可由漂变固定 |
| **分子钟** | Molecular Clock | 中性突变的替换速率恒定（K=u），可用于估计进化时间 |
| **替换负荷** | Substitutional Load | Haldane提出，有利等位基因替换带来的适合度代价 |
| **Wright-Fisher模型** | Wright-Fisher Model | 描述有限种群中等位基因频率世代间随机变化的基本模型 |
| **抽样误差** | Sampling Error | 从有限种群中随机选取配子/亲本时产生的频率偏差 |

---

## 🔮 下节预告

### Day 55 · 迁移与基因流（Migration & Gene Flow）

明天的学习主题是**迁移与基因流**。我们将探讨：

- 基因流如何抵消遗传漂变和自然选择的作用
- 迁移率对种群间遗传分化的影响
- Wright的岛屿模型与 stepping-stone 模型
- 人类迁徙历史与基因流
- 基因流在物种形成与保护生物学中的意义

基因流是维持种群遗传多样性的重要机制，也是理解群体遗传学不可或缺的一环。敬请期待！

---

## 🔗 学习资源链接汇总

| 类型 | 资源名称 | 链接 |
|------|----------|------|
| 🌐 Wikipedia | Genetic Drift（英文） | [en.wikipedia.org/wiki/Genetic_drift](https://en.wikipedia.org/wiki/Genetic_drift) |
| 🌐 Wikipedia | 遗传漂变（中文） | [zh.wikipedia.org/wiki/遗传漂变](https://zh.wikipedia.org/wiki/遗传漂变) |
| 🌐 Wikipedia | Sewall Wright | [en.wikipedia.org/wiki/Sewall_Wright](https://en.wikipedia.org/wiki/Sewall_Wright) |
| 🌐 Wikipedia | Motoo Kimura | [en.wikipedia.org/wiki/Motoo_Kimura](https://en.wikipedia.org/wiki/Motoo_Kimura) |
| 🌐 Wikipedia | Lonesome George | [en.wikipedia.org/wiki/Lonesome_George](https://en.wikipedia.org/wiki/Lonesome_George) |
| 📚 NCBI | Gene in Populations | [ncbi.nlm.nih.gov/books/NBK21122](https://www.ncbi.nlm.nih.gov/books/NBK21122/) |
| 📚 NCBI PMC | 木村资生中性理论回顾 | [pmc.ncbi.nlm.nih.gov/articles/PMC1203127](https://pmc.ncbi.nlm.nih.gov/articles/PMC1203127/pdf/183.pdf) |
| 📚 NCBI PMC | 遗传漂变教学反思 | [pmc.ncbi.nlm.nih.gov/articles/PMC10285527](https://pmc.ncbi.nlm.nih.gov/articles/PMC10285527/) |
| 🎓 Khan Academy | Genetic Drift | [khanacademy.org](https://en.khanacademy.org/science/biology/her/heredity-and-genetics/a/genetic-drift-founder-bottleneck) |
| 🎬 JoVE | Genetic Drift（中文） | [jove.com](https://www.jove.com/cn/science-education/v/11128/genetic-drift) |
| 📖 Stanford | Genetic Drift 哲学综述 | [plato.stanford.edu](https://plato.stanford.edu/entries/genetic-drift/) |

---

*遗传学100天学习计划 · Day 54 · 遗传漂变*
*自动生成于 2026年7月7日*
