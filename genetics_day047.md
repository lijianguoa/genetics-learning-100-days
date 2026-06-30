# 遗传学100天学习计划 · Day 47

## 多基因遗传（Polygenic Inheritance）

> **学习日期**: 2026年6月30日 · Day 47
> **所属部分**: 第五部分 · 经典遗传学发展（Day 46-60）
> **上期回顾**: [Day 46 · 经典遗传学的形成背景](genetics_day046.md)
> **下期预告**: [Day 48 · 数量遗传学基础](genetics_day048.md)

---

## 一、配图

### 图1：多基因遗传的加性效应模型
![多基因遗传加性效应模型](genetics_images/day047/polygenic_inheritance_model.png)

*图解：展示多基因遗传中多个微效基因的累加效应如何产生连续变异分布。以人类身高为例，每个增效等位基因贡献微小增量，随着基因对数增多，F2代表型分布从离散的二项分布逐渐趋近连续的正态分布（钟形曲线）。*

### 图2：Nilsson-Ehle小麦籽粒颜色实验
![Nilsson-Ehle实验](genetics_images/day047/nilsson_ehle_experiment.png)

*图解：Nilsson-Ehle 1909年经典小麦籽粒颜色实验示意图。展示深红×白色杂交后F1代（中间红色）和F2代的分离比：两对基因模型下呈1:4:6:4:1的5级分布；三对基因模型下呈1:6:15:20:15:6:1的7级分布。颜色梯度直观展示多基因的等加性效应。*

---

## 二、历史背景

### 生物统计学派与孟德尔学派的大论战

20世纪初，遗传学界分裂为两大阵营，爆发了持续十余年的激烈争论：

- **孟德尔学派**（Mendelians）：以William Bateson为代表，坚持所有遗传现象都可以用孟德尔的离散遗传因子来解释，性状变异是"非此即彼"的。
- **生物统计学派**（Biometricians）：以Francis Galton和Karl Pearson为代表，通过大规模人体测量（身高、体重等）发现这些性状呈**连续变异**（continuous variation），而非离散分类，认为连续变异无法用孟德尔定律解释。

这场争论的本质是：**连续变异是否具有遗传基础？孟德尔因子能否解释连续性状？**

1908-1909年间，瑞典遗传学家Nilsson-Ehle的小麦实验和1918年Fisher的数学证明，最终为这场争论画上了句号——**孟德尔遗传完全可以解释连续变异**，关键在于多个微效基因的累加效应。

> 📚 **延伸阅读**：
> - [维基百科：Polygenic Inheritance](https://en.wikipedia.org/wiki/Polygenic_inheritance)
> - [PMC：From R.A. Fisher's 1918 Paper to GWAS a Century Later](https://pmc.ncbi.nlm.nih.gov/articles/PMC6456325/)

---

## 三、核心概念

### 3.1 什么是多基因遗传？

**多基因遗传**（Polygenic Inheritance），又称**多因子遗传**（Multifactorial Inheritance），是指一个表型性状由**多个基因**（通常数十到数千个）共同控制的遗传方式。每个基因对表型的单独效应很小（称为**微效基因**），但这些效应可以通过**累加**共同决定最终表型。

### 3.2 多基因遗传 vs 孟德尔单基因遗传

| 对比维度 | 孟德尔单基因遗传 | 多基因遗传 |
|---------|-----------------|----------|
| 控制基因数量 | 1-2个主效基因 | 多个微效基因（可多达数百上千） |
| 表型变异类型 | **离散变异**（如黄色/绿色豌豆） | **连续变异**（如身高150-200cm） |
| 环境影响 | 很小或可忽略 | **显著**（环境修饰基因表达） |
| F2代分离比 | 典型孟德尔比（3:1, 9:3:3:1） | 趋近**正态分布**（钟形曲线） |
| 统计分析方法 | 卡方检验 | 方差分析（ANOVA）、遗传力估算等 |
| 经典实例 | 豌豆颜色、血型、镰刀型贫血 | 身高、肤色、体重、智力、疾病风险 |

### 3.3 加性基因效应（Additive Gene Action）

多基因遗传的核心机制是**等加性效应**：

- 每个增效等位基因（contributing allele）对表型贡献**等量**的微小增量
- 效应可以**线性累加**——拥有越多增效等位基因，表型值越高
- 减效等位基因（non-contributing allele）不增加表型值
- 杂合子与纯合子的差异遵循剂量效应

**数学表达**：若每个增效等位基因增加效应值 `a`，则含有 `k` 个增效等位基因的个体的表型值为：
```
P = P₀ + k × a + e
```
其中 `P₀` 为基础表型值，`a` 为单基因效应值，`e` 为环境效应。

### 3.4 连续变异与正态分布

当涉及**大量基因对**（n对）时，F2代的表型分布遵循二项展开 `(a+b)^(2n)`：

- n=1对基因 → 3个表型类别（1:2:1）
- n=2对基因 → 5个表型类别（1:4:6:4:1）
- n=3对基因 → 7个表型类别（1:6:15:20:15:6:1）
- n=10对基因 → 21个表型类别（趋近正态分布）
- n→∞ → **连续正态分布**（钟形曲线）

加上环境因素的随机修饰，现实中大多数多基因性状呈现经典的**正态分布**。

### 3.5 阈值性状（Threshold Traits）

某些多基因性状在遗传层面是连续的，但在表型观察层面表现为**离散的"有/无"**分类：

- 当多基因风险积累超过某个**阈值**时，个体才表现出该性状
- **实例**：先天性唇腭裂、糖尿病、高血压、精神分裂症
- 携带风险基因越多（遗传负荷越大），越接近阈值，发病风险越高
- 环境因素可以推动个体越过阈值

> 📚 **延伸学习**：
> - [维基百科：Quantitative Genetics](https://en.wikipedia.org/wiki/Quantitative_genetics)
> - [Khan Academy：Polygenic Inheritance](https://www.khanacademy.org/science/up-class-12th-biology/xd64b9ea553b83790:4-principles-of-inheritance-and-variation/xd64b9ea553b83790:polygenic-inheritance-pleiotropy-and-sex-determination/v/polygenic-inheritance)
> - [B站：复旦大学遗传学课程 - 多基因遗传](https://www.bilibili.com/opus/648482882987229208)

---

## 四、科学家故事

### 🌾 Herman Nilsson-Ehle（1873–1949）——多基因遗传的实验奠基人

Nilsson-Ehle出生于瑞典一个农民家庭，对植物育种有浓厚兴趣。他在隆德大学（Lund University）师从著名植物学家，致力于谷物遗传研究。

1909年，他在小麦籽粒颜色的杂交实验中做出了划时代发现：

**实验灵感**：前人已经注意到小麦籽粒颜色深浅不一，但没有人系统研究过其遗传规律。Nilsson-Ehle选择了红色与白色籽粒的纯系品种进行杂交。

**关键发现**：
- 某些杂交组合中，F2代不是简单的3:1或9:3:3:1分离
- 而是出现了**中间颜色**，呈现连续的梯度分布
- 进一步分析发现，F2代分离比符合 **1:4:6:4:1**（两对基因）或 **1:6:15:20:15:6:1**（三对基因）

他大胆提出**多因子假说**：同一性状可以由多对独立的孟德尔因子控制，各因子的效应微小且大致相等，效应可以累加。

这一发现的意义在于——它**首次用实验证据**证明了连续变异可以用孟德尔遗传原理来解释，为终结孟德尔学派与生物统计学派的论战奠定了实验基础。

---

### 📊 Ronald Aylmer Fisher（1890–1962）——统一遗传学的大师

Fisher是20世纪最伟大的统计学家和遗传学家之一。他1918年发表的论文被公认为**数量遗传学的奠基之作**。

**天才青年**：Fisher天赋异禀，视力极差（看不清黑板上的数学公式），却凭借超强的几何直觉完成了许多数学证明。他在剑桥大学学习数学和物理时，对生物统计学产生了浓厚兴趣。

**1918年论文的诞生背景**：
- 当时孟德尔学派（Bateson）和生物统计学派（Pearson）的争论已持续十余年
- Pearson公开嘲讽孟德尔定律无法解释连续变异
- Fisher年仅28岁，发表了一篇35页的论文，用严密的数学证明**终结了这场争论**

**论文的核心贡献**：
1. 证明了若数量性状受大量孟德尔因子控制，每个因子效应微小，则群体表型分布趋近正态
2. 首次引入统计学中"**方差**"（variance）的概念
3. 创立了**方差分析**（ANOVA）方法
4. 将遗传方差分解为**加性方差**（V_A）和**显性方差**（V_D）
5. 推导了各种亲缘关系（亲子、兄弟姐妹、半同胞等）之间的理论相关系数

这篇论文不仅统一了两大遗传学派，还创立了**方差分析**这一今天所有科学领域都在使用的统计方法。

> 📚 **延伸阅读**：
> - [维基百科：Ronald Fisher](https://en.wikipedia.org/wiki/Ronald_Fisher)
> - [维基百科：Nilsson-Ehle](https://en.wikipedia.org/wiki/Nilsson-Ehle)

---

## 五、重要文献

### 📄 经典论文列表

| 年份 | 作者 | 论文/著作 | 核心贡献 |
|------|------|----------|--------|
| 1909 | Nilsson-Ehle, H. | Kreuzungsuntersuchungen an Hafer und Weizen. *Lunds Universitets Årsskrift* | 多因子假说的奠基性实验 |
| 1910 | East, E.M. | 烟草花冠长度杂交实验 | 独立验证多基因遗传理论 |
| 1918 | Fisher, R.A. | The Correlation between Relatives on the Supposition of Mendelian Inheritance. *Trans. R. Soc. Edinb.* 52(2): 399-433 | 统一孟德尔遗传与连续变异，创立方差分析 |
| 1921 | Wright, S. | Systems of Mating. *Genetics* 6: 111-178 | 近交系数与亲缘系数方法 |
| 1930 | Fisher, R.A. | *The Genetical Theory of Natural Selection* | 自然选择基本定理 |
| 1931 | Wright, S. | Evolution in Mendelian Populations. *Genetics* 16: 97-159 | 群体遗传学奠基文献 |
| 1937 | Lush, J.L. | *Animal Breeding Plans* | 数量遗传学应用于动物育种 |
| 1941 | Mather, K. | Variation and Selection of Polygenic Characters. *J. Genetics* 41: 159-193 | 首次提出"polygenes"术语 |
| 2020 | Crouch & Bodmer | Polygenic inheritance, GWAS, polygenic risk scores... *PNAS* 117(32): 18924-18933 | 多基因遗传百年发展综述 |

> 📚 **在线阅读**：
> - [PMC: Fisher 1918 to GWAS a Century Later](https://pmc.ncbi.nlm.nih.gov/articles/PMC6456325/)
> - [PMC: Common Disease Polygenicity](https://pmc.ncbi.nlm.nih.gov/articles/PMC9945947/)
> - [PMC: Complex Trait Genetic Architecture](https://pmc.ncbi.nlm.nih.gov/articles/PMC9053444/)
> - [NCBI Bookshelf: From Common Variant to Function](https://www.ncbi.nlm.nih.gov/books/NBK609758/?report=reader)

---

## 六、经典实验

### 🔬 Nilsson-Ehle小麦籽粒颜色实验（1909）——多基因遗传的经典证明

**实验材料**：
- 纯系深红色籽粒小麦品种（P₁）
- 纯系白色籽粒小麦品种（P₂）

**实验步骤与结果**：

**第一组：两对基因模型（AaBb）**
```
P₁: AABB（深红） × aabb（白色）
F₁: AaBb（中间红色）—— 全部一致
F₁ × F₁ → F₂:
  深红(AABB): 1/16
  中深红: 4/16
  中间红: 6/16
  中浅红: 4/16
  白色(aabb): 1/16
  → 比例 = 1:4:6:4:1（5个等级）
```

**第二组：三对基因模型（AaBbCc）**
```
F₂分布:
  深红(AABBCC): 1/64
  6个中间等级: 6/64, 15/64, 20/64, 15/64, 6/64
  白色(aabbcc): 1/64
  → 比例 = 1:6:15:20:15:6:1（7个等级）
```

**关键洞察**：
- 每个红色等位基因（A、B、C）贡献等量红色素
- 白色等位基因（a、b、c）不贡献色素
- 颜色深浅 = 增效等位基因的**累加数量**
- 基因对数越多 → 表型等级越多 → 越趋近连续分布

---

### 🔬 Fisher 1918年数学分析——连续变异的遗传统一

Fisher并未做实验，而是用纯数学方法完成了这一划时代工作：

**核心论证**：
1. 假设一个数量性状受 n 个独立的孟德尔因子控制
2. 每个因子有两个等位基因，效应差为 ε（极小）
3. 根据中心极限定理，当 n 足够大时，表型分布趋近正态分布
4. 推导了各种亲缘关系的理论相关系数（如父子r=0.5，全同胞r=0.5，半同胞r=0.25）

**方差分解公式**：
```
V_P = V_A + V_D + V_E

其中：
V_P = 表型总方差
V_A = 加性遗传方差（决定选择响应）
V_D = 显性方差（杂合优势贡献）
V_E = 环境方差
```

> 📚 **延伸学习**：
> - [B站：多基因假说详解](https://www.bilibili.com/read/cv6763015/)
> - [NCBI Bookshelf: Genetics of Type 2 Diabetes](https://www.ncbi.nlm.nih.gov/books/NBK567998/)

---

## 七、小故事

### 📖 "一篇论文终结一场战争"

1918年，年轻的Fisher将他的论文提交给Karl Pearson主编的《Biometrika》杂志。Pearson——生物统计学派的领袖、这场争论的核心人物——拒绝发表这篇旨在推翻自己观点的论文。

最终，这篇论文发表在《爱丁堡皇家学会学报》（Transactions of the Royal Society of Edinburgh）上。讽刺的是，正是Pearson的拒绝，迫使Fisher将论文写得更加完整和严谨，反而成就了这篇百年经典。

据说Pearson后来读了Fisher的论文，久久无言。一位同时代的科学家评论道："Fisher用一支笔和一叠纸，做了孟德尔学派和生物统计学派用十几年实验都没能做到的事。"

---

### 📖 小麦颜色的"密码"

Nilsson-Ehle在实验中注意到一个有趣的现象：不同的小麦品种中，有些杂交后代只有3个颜色等级（1:2:1），有些有5个等级（1:4:6:4:1），有些有7个等级（1:6:15:20:15:6:1）。

他恍然大悟——这不是实验误差，而是不同品种中**控制籽粒颜色的基因对数不同**！有的品种只有1对基因，有的有2对，有的有3对。参与基因越多，颜色分级就越细，越接近连续的梯度。

这个看似简单的发现，实际上揭示了遗传学中一个深刻原理：**同一性状在不同物种或品种中，可以由不同数量的基因控制**。这一原理至今仍是遗传学研究的重要参考。

---

## 八、思考题

### 🧠 基础题

1. **概念辨析**：多基因遗传与多效性（pleiotropy）有什么区别？请各举一例说明。

2. **数学推导**：在3对独立基因控制下，F2代中拥有恰好4个增效等位基因的个体占多大比例？（提示：考虑二项展开的各项系数）

3. **现实联系**：人类身高通常呈正态分布。如果一个人的父母都很高，但这个人却较矮，请用多基因遗传的原理解释这一现象。

### 🧠 进阶题

4. **方差分解**：已知某多基因性状的表型方差V_P=100，其中加性遗传方差V_A=40，显性方差V_D=10，环境方差V_E=50。请计算广义遗传力（H²）和狭义遗传力（h²），并解释两者的区别。

5. **阈值模型**：为什么唇腭裂在男性中的发病率高于女性？请用阈值性状模型解释性别差异对发病风险的影响。

6. **历史思考**：Fisher 1918年的论文为什么能"终结一场战争"？它具体解决了孟德尔学派与生物统计学派的哪些争议？

> 📚 **参考资源**：
> - [维基百科：Heritability](https://en.wikipedia.org/wiki/Heritability)
> - [GWAS Catalog](https://www.ebi.ac.uk/gwas/docs/related-resources)

---

## 九、术语表

| 中文术语 | 英文术语 | 简要定义 |
|---------|---------|--------|
| 多基因遗传 | Polygenic Inheritance | 多个微效基因共同控制一个表型性状的遗传方式 |
| 多因子遗传 | Multifactorial Inheritance | 多基因遗传的同义术语，强调基因与环境的共同作用 |
| 微效基因 | Minor Gene / Polygene | 单独效应很小的基因，大量微效基因累加产生显著表型效应 |
| 主效基因 | Major Gene | 效应较大、可单独检测到的基因（与微效基因相对） |
| 加性效应 | Additive Effect | 等位基因效应可线性累加，无显性或上位性交互 |
| 加性遗传方差 | Additive Genetic Variance (V_A) | 育种值的方差，决定亲代与子代的相似程度及选择响应 |
| 显性方差 | Dominance Variance (V_D) | 杂合子偏离纯合子中值的方差成分 |
| 上位性 | Epistasis | 不同基因座之间的非加性交互效应 |
| 连续变异 | Continuous Variation | 性状在群体中呈连续分布，无法明确分类 |
| 离散变异 | Discontinuous Variation | 性状可分为有限几个明确类别 |
| 正态分布 | Normal Distribution | 钟形曲线，多基因性状在群体中的典型分布 |
| 阈值性状 | Threshold Trait | 潜层面连续但超过阈值后表现为离散分类的性状 |
| 数量性状位点 | Quantitative Trait Locus (QTL) | 基因组中影响数量性状的区域 |
| 遗传力 | Heritability | 表型变异中归因于遗传变异的比例 |
| 无穷小模型 | Infinitesimal Model | Fisher提出的假设：大量基因各具极小效应 |
| 方差分析 | ANOVA | Fisher首创的统计方法，将总变异分解为各成分 |
| 多基因风险评分 | Polygenic Risk Score (PRS) | 汇总多个变异效应评估个体疾病风险的工具 |

---

## 十、下节预告

### Day 48 · 数量遗传学基础

在Day 47中，我们了解了多基因遗传的基本概念和历史发现。Day 48将深入**数量遗传学**的系统理论框架：

- **方差组分模型**：V_P = V_A + V_D + V_I + V_E 的完整分解
- **遗传力的估算方法**：狭义遗传力 h² 与广义遗传力 H²
- **亲属相关分析**：利用半同胞、全同胞、双胞胎数据估算遗传参数
- **育种值与选择响应**：Breeder's Equation R = h²S
- **数量遗传学在现代育种和医学中的应用**

数量遗传学正是从多基因遗传理论中生长出来的重要分支，是理解复杂性状遗传规律的关键工具。

> 📖 **预习资源**：
> - [NCBI Bookshelf: Contextualizing Convergent Common Variant Mechanisms](https://www.ncbi.nlm.nih.gov/books/NBK609763/)
> - [B站：医学遗传学·多基因遗传病](https://www.bilibili.com/opus/1087073995206950933)

---

## 📚 综合学习资源

### 🎬 视频资源
- [Khan Academy: Polygenic Inheritance](https://www.khanacademy.org/science/up-class-12th-biology/xd64b9ea553b83790:4-principles-of-inheritance-and-variation/xd64b9ea553b83790:polygenic-inheritance-pleiotropy-and-sex-determination/v/polygenic-inheritance)
- [B站：复旦大学遗传学课程](https://www.bilibili.com/opus/648482882987229208)
- [B站：遗传学0基础速成](https://www.bilibili.com/video/BV1EKjh6tEv6/)

### 📖 文献与数据库
- [Wikipedia: Polygenic Inheritance](https://en.wikipedia.org/wiki/Polygenic_inheritance)
- [Wikipedia: Ronald Fisher](https://en.wikipedia.org/wiki/Ronald_Fisher)
- [PMC: Fisher 1918 to GWAS](https://pmc.ncbi.nlm.nih.gov/articles/PMC6456325/)
- [GWAS Catalog (EBI)](https://www.ebi.ac.uk/gwas/docs/related-resources)

---

*本文由遗传学100天学习计划自动生成 · Day 47 / 100*
*最后更新：2026-06-30*