# Day 88：基因编辑技术（Gene Editing Technology）

> **遗传学100天学习计划** | 第七部分：现代遗传学（Day 81-95）  
> **日期**：2026年8月10日 | **Day 88/100**  
> **主题**：基因编辑技术——从锌指核酸酶到CRISPR-Cas9再到引物编辑  
> **难度**：★★★★☆ | **预计学习时间**：45-60分钟

---

## 📷 配图

![CRISPR-Cas9基因编辑机制示意图](gene_editing_day088_01.jpg)  
*图1：CRISPR-Cas9系统工作原理——Cas9蛋白在sgRNA引导下识别并切割靶DNA序列*

![基因编辑技术发展时间线](gene_editing_day088_02.jpg)  
*图2：基因编辑技术演进历程——从ZFN到引物编辑的25年技术迭代*

---

## 📜 历史背景

基因编辑技术是指利用工程化工具对生物体基因组进行定点修饰的技术。其发展历程可概括为三代技术迭代与两次范式革命。

### 第一代：锌指核酸酶（ZFN）时代（1996-2010）

锌指核酸酶（Zinc Finger Nuclease, ZFN）是最早被开发的可编程基因编辑工具。1996年，Johns Hopkins大学的Srinivasan Chandrasegaran团队首次将锌指蛋白的DNA识别结构域与FokI核酸酶切割结构域融合，创建了人工核酸酶。2005年，Sangamo Biosciences的Urnov等人首次在人类细胞中实现了高效的基因校正（[Urnov et al., Nature, 2005](https://pubmed.ncbi.nlm.nih.gov/15892197/)）。ZFN的局限在于蛋白质工程复杂、成本高昂且脱靶率较高。

- **Wikipedia**: [Zinc Finger Nuclease](https://en.wikipedia.org/wiki/Zinc_finger_nuclease)
- **NCBI综述**: [The Basic Science of Genome Editing](https://www.ncbi.nlm.nih.gov/books/NBK447276/)

### 第二代：TALEN时代（2010-2012）

转录激活因子样效应物核酸酶（TALEN）于2010年由Christian等人开发（[Christian et al., Genetics, 2010](https://pubmed.ncbi.nlm.nih.gov/20660643/)），2011年Miller等人进一步优化（[Miller et al., Nature Biotechnology, 2011](https://pubmed.ncbi.nlm.nih.gov/21179091/)）。TALEN比ZFN更易设计、特异性更高，但仍需为每个靶点定制蛋白质，工作量巨大。

- **Wikipedia**: [TALEN](https://en.wikipedia.org/wiki/TALEN)

### 第三代：CRISPR-Cas9革命（2012至今）

CRISPR（Clustered Regularly Interspaced Short Palindromic Repeats）系统源自细菌的适应性免疫系统。2007年，Barrangou等人在*Streptococcus thermophilus*中首次实验证明CRISPR提供抗噬菌体免疫（[Barrangou et al., Science, 2007](https://pubmed.ncbi.nlm.nih.gov/17379808/)）。2012年，Jennifer Doudna和Emmanuelle Charpentier在里程碑式论文中证明Cas9可被RNA引导切割DNA（[Jinek et al., Science, 2012](https://pubmed.ncbi.nlm.nih.gov/22745249/)）。2013年，张锋团队和George Church团队分别独立实现CRISPR-Cas9在人类细胞中的基因组编辑（[Cong et al., Science, 2013](https://pubmed.ncbi.nlm.nih.gov/23287718/); [Mali et al., Science, 2013](https://pubmed.ncbi.nlm.nih.gov/23287722/)），从此开启了基因编辑的新纪元。

- **Wikipedia (英文)**: [CRISPR gene editing](https://en.wikipedia.org/wiki/CRISPR_gene_editing) | [CRISPR](https://en.wikipedia.org/wiki/CRISPR)
- **Wikipedia (中文)**: [CRISPR](https://zh.wikipedia.org/wiki/CRISPR) | [基因编辑](https://zh.wikipedia.org/wiki/基因编辑)
- **B站教学**: [CRISPR-Cas9基因编辑技术基本概念及原理](https://www.bilibili.com/video/BV1Pmm5BeE68/)
- **YouTube**: [Jennifer Doudna讲解CRISPR](https://www.youtube.com/watch?v=SuAxDVBt7kQ) | [CRISPR-Cas9动画演示](https://www.youtube.com/watch?v=2pp7E5-X1Ek)

### 范式革命：碱基编辑与引物编辑（2016-2019）

David R. Liu（刘如谦）团队于2016年发明碱基编辑技术（[Komor et al., Nature, 2016](https://pubmed.ncbi.nlm.nih.gov/27096365/)），2017年扩展至ABE（[Gaudelli et al., Nature, 2017](https://pubmed.ncbi.nlm.nih.gov/29160308/)），2019年发明引物编辑（[Anzalone et al., Nature, 2019](https://pubmed.ncbi.nlm.nih.gov/31634902/)），实现了"搜索-替换"式的精准编辑，无需双链断裂。

- **Wikipedia**: [Base editing](https://en.wikipedia.org/wiki/Base_editing) | [Prime editing](https://en.wikipedia.org/wiki/Prime_editing)
- **David Liu论文列表**: [Key Publications](https://www.liugroup.us/key-publications-2/)

---

## 🧬 核心概念

### 1. CRISPR-Cas9系统的工作原理

CRISPR-Cas9系统由三个核心组件构成：

| 组件 | 全称 | 功能 |
|------|------|------|
| **Cas9** | CRISPR-associated protein 9 | 核酸内切酶，含HNH和RuvC两个结构域，分别切割DNA的互补链和非互补链 |
| **sgRNA** | Single Guide RNA | 由crRNA和tracrRNA融合而成，负责识别靶DNA序列（5'-NGG-3' PAM上游约20bp） |
| **PAM** | Protospacer Adjacent Motif | 靶DNA上的NGG序列，Cas9识别和切割的必要条件 |

**切割与修复机制**：
- Cas9在PAM上游3bp处产生平末端双链断裂（DSB）
- 细胞通过两种途径修复：
  - **NHEJ（非同源末端连接）**：易出错，产生indel（插入/缺失），用于基因敲除
  - **HDR（同源定向修复）**：精确修复，需供体DNA模板，用于基因敲入

- **诺贝尔奖2020化学奖科学背景文档**: [PDF](https://www.nobelprize.org/uploads/2020/10/advanced-chemistryprize2020.pdf)
- **Broad Institute CRISPR问答**: [Q&A](https://www.broadinstitute.org/what-broad/areas-focus/project-spotlight/questions-and-answers-about-crispr)

### 2. 碱基编辑（Base Editing）

碱基编辑无需产生双链断裂，直接进行单碱基转换：

| 编辑器 | 转换 | 结构 | 发明年份 |
|--------|------|------|----------|
| **CBE** | C→T (G→A) | nCas9(D10A) + 胞嘧啶脱氨酶(APOBEC1) | 2016 |
| **ABE** | A→G (T→C) | nCas9(D10A) + 进化版TadA脱氨酶 | 2017 |

- **Wikipedia**: [Base editing](https://en.wikipedia.org/wiki/Base_editing)

### 3. 引物编辑（Prime Editing）

引物编辑是当前最先进的精准编辑技术：

- **结构**：Cas9(H840A) nickase + 工程化逆转录酶（M-MLV RT）
- **向导RNA**：pegRNA（Prime Editing Guide RNA），含PBS（引物结合位点）和RTT（逆转录模板）
- **能力**：可实现全部12种碱基转换 + 小片段插入/缺失
- **意义**：理论上可纠正约89%的已知致病变异

- **Wikipedia**: [Prime editing](https://en.wikipedia.org/wiki/Prime_editing)
- **PMC全文**: [Anzalone et al., 2019](https://pmc.ncbi.nlm.nih.gov/articles/PMC6907074/)

### 4. 脱靶效应（Off-target Effects）

脱靶效应是基因编辑技术面临的核心安全挑战。Cas9可能在非靶标位点产生意外切割，导致基因组不稳定甚至癌症风险。降低脱靶的策略包括：高保真Cas9变体（eSpCas9、SpCas9-HF1）、优化sgRNA设计、双nickase策略等。

- **PMC综述**: [Recent advances in therapeutic CRISPR-Cas9](https://pmc.ncbi.nlm.nih.gov/articles/PMC10080534/)

---

## 👨‍🔬 科学家故事

### 珍妮弗·杜德纳（Jennifer A. Doudna）

杜德纳现任加州大学伯克利分校教授、Howard Hughes Medical Institute研究员。她自研究生阶段起专注于RNA结构生物学研究。2011年，在波多黎各的一次学术会议上，她结识了Emmanuelle Charpentier。两人决定合作研究*Streptococcus pyogenes*中CRISPR-Cas系统的机制。2012年，她们在*Science*发表了里程碑论文（[Jinek et al., 2012](https://pubmed.ncbi.nlm.nih.gov/22745249/)），证明Cas9可被单一引导RNA编程切割任意DNA序列。这项工作奠定了CRISPR基因编辑的基础。2020年，杜德纳与Charpentier共同获得诺贝尔化学奖。

- **Wikipedia (英文)**: [Jennifer Doudna](https://en.wikipedia.org/wiki/Jennifer_Doudna)
- **Wikipedia (中文)**: [珍妮弗·杜德纳](https://zh.wikipedia.org/wiki/珍妮弗·杜德纳)
- **实验室出版物**: [Doudna Lab Publications](https://doudnalab.org/publications/)

### 埃马纽埃尔·沙尔庞捷（Emmanuelle Charpentier）

Charpentier现任马克斯·普朗克病原体科学研究所所长。她在研究*Streptococcus pyogenes*的RNA生物学时，发现了tracrRNA分子——它是CRISPR/Cas系统中RNA加工的关键组分（[Deltcheva et al., Nature, 2011](https://pubmed.ncbi.nlm.nih.gov/21455174/)）。她与Doudna的合作最终促成了2012年的奠基性论文。Charpentier的科研生涯充满曲折，曾在多个国家和机构辗转，但她始终坚持对基础科学的好奇心。2020年，她与Doudna成为科学史上首次全女性获得诺贝尔科学奖项的组合。

- **Wikipedia (英文)**: [Emmanuelle Charpentier](https://en.wikipedia.org/wiki/Emmanuelle_Charpentier)
- **Wikipedia (中文)**: [埃马纽埃尔·沙尔庞捷](https://zh.wikipedia.org/wiki/埃马纽埃尔·沙尔庞捷)

### 张锋（Feng Zhang）

张锋现任MIT教授、Broad Institute核心成员、McGovern Institute研究员。2013年1月，张锋团队率先在人类和小鼠细胞中实现CRISPR-Cas9基因编辑（[Cong et al., Science, 2013](https://pubmed.ncbi.nlm.nih.gov/23287718/)），这是该领域被引用最多的论文。张锋团队还开发了多种CRISPR工具扩展，包括CRISPRa/CRISPRi基因调控系统、光控基因编辑系统等。他与Doudna团队之间关于CRISPR专利的争议持续多年，最终美国专利商标局裁定Broad Institute胜出（关于真核细胞应用的权利）。

- **Wikipedia (英文)**: [Feng Zhang](https://en.wikipedia.org/wiki/Feng_Zhang)
- **Wikipedia (中文)**: [张锋 (生物学家)](https://zh.wikipedia.org/wiki/张锋_(生物学家))
- **Broad Institute研究亮点**: [CRISPR Research Highlights](https://www.broadinstitute.org/research-highlights-crispr)

### 刘如谦（David R. Liu）

刘如谦现任哈佛大学教授、Broad Institute研究员、Howard Hughes Medical Institute研究员。他开创了"无断裂编辑"的新范式：2016年发明CBE（胞嘧啶碱基编辑器），2017年发明ABE（腺嘌呤碱基编辑器），2019年发明引物编辑。这些技术使基因编辑从"剪刀"时代进入"搜索-替换"时代。引物编辑理论上可纠正人类已知致病变异的89%，被视为基因治疗领域的革命性突破。

- **Wikipedia (英文)**: [David R. Liu](https://en.wikipedia.org/wiki/David_R._Liu)
- **关键论文列表**: [Liu Group Key Publications](https://www.liugroup.us/key-publications-2/)

---

## 📚 重要文献

| # | 论文 | 期刊 | 年份 | PMID | 意义 |
|---|------|------|------|------|------|
| 1 | Barrangou R, et al. "CRISPR provides acquired resistance against viruses in prokaryotes" | Science 315:1709-1712 | 2007 | [17379808](https://pubmed.ncbi.nlm.nih.gov/17379808/) | 首次实验证明CRISPR是细菌免疫系统 |
| 2 | Deltcheva E, et al. "CRISPR RNA maturation by trans-encoded small RNA and host factor RNase III" | Nature 471:602-607 | 2011 | [21455174](https://pubmed.ncbi.nlm.nih.gov/21455174/) | 发现tracrRNA |
| 3 | **Jinek M, Chylinski K, Fonfara I, Hauer M, Doudna JA, Charpentier E.** "A programmable dual-RNA-guided DNA endonuclease in adaptive bacterial immunity" | Science 337:816-821 | 2012 | **[22745249](https://pubmed.ncbi.nlm.nih.gov/22745249/)** | **奠基性论文**：Cas9可被RNA引导切割DNA |
| 4 | **Cong L, Ran FA, Cox D, ... Zhang F.** "Multiplex genome engineering using CRISPR/Cas systems" | Science 339:819-823 | 2013 | **[23287718](https://pubmed.ncbi.nlm.nih.gov/23287718/)** | 首次在人类细胞实现CRISPR编辑 |
| 5 | Mali P, ... Church GM. "RNA-guided human genome engineering via Cas9" | Science 339:823-826 | 2013 | [23287722](https://pubmed.ncbi.nlm.nih.gov/23287722/) | Church团队同期实现人类细胞CRISPR编辑 |
| 6 | Doudna JA, Charpentier E. "The new frontier of genome engineering with CRISPR-Cas9" | Science 346:1258096 | 2014 | [25299471](https://pubmed.ncbi.nlm.nih.gov/25299471/) | 权威综述 |
| 7 | **Komor AC, ... Liu DR.** "Programmable editing of a target base in genomic DNA without double-stranded DNA cleavage" | Nature 533:420-424 | 2016 | **[27096365](https://pubmed.ncbi.nlm.nih.gov/27096365/)** | **碱基编辑诞生**（CBE） |
| 8 | **Gaudelli NM, ... Liu DR.** "Programmable base editing of A•T to G•C in genomic DNA without DNA cleavage" | Nature 551:464-471 | 2017 | **[29160308](https://pubmed.ncbi.nlm.nih.gov/29160308/)** | **ABE诞生** |
| 9 | **Anzalone AV, ... Liu DR.** "Search-and-replace genome editing without double-strand breaks or donor DNA" | Nature 576:149-157 | 2019 | **[31634902](https://pubmed.ncbi.nlm.nih.gov/31634902/)** | **引物编辑诞生** |

### PMC全文链接（免费获取）
- Jinek 2012全文: [PMC6286148](https://pmc.ncbi.nlm.nih.gov/articles/PMC6286148/)
- Cong 2013全文: [PMC3795411](https://pmc.ncbi.nlm.nih.gov/articles/PMC3795411/)
- Anzalone 2019全文: [PMC6907074](https://pmc.ncbi.nlm.nih.gov/articles/PMC6907074/)

### 综述文献
- [Advancing CRISPR genome editing into gene therapy clinical trials (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC12094669/)
- [A CRISPR view of the 2020 Nobel Prize in Chemistry (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC7773339/)
- [NHGRI: Editing The Book Of Life With Molecular Scissors](https://www.genome.gov/editing-the-book-of-life-with-molecular-scissors)

---

## 🔬 经典实验

### 实验一：CRISPR免疫功能验证（Barrangou et al., 2007）

在*Streptococcus thermophilus*中，研究者通过人工添加或删除特定的CRISPR间隔序列（spacer），改变了细菌对噬菌体的抗性表型。含有匹配间隔序列的细菌能抵抗对应噬菌体感染，而不含有的则被杀死。这首次证明CRISPR-Cas系统是细菌的适应性免疫系统。

- **论文**: [Barrangou et al., 2007](https://pubmed.ncbi.nlm.nih.gov/17379808/)

### 实验二：Cas9体外编程切割DNA（Jinek et al., 2012）

Doudna和Charpentier在体外系统中证明：纯化的Cas9蛋白在tracrRNA:crRNA双RNA引导下，可在特定位点切割双链DNA。关键突破是将双RNA融合为单链嵌合体（sgRNA），使整个系统简化为"一个蛋白+一条RNA"。这一简化奠定了基因组编辑工具的基础。

- **论文**: [Jinek et al., 2012](https://pubmed.ncbi.nlm.nih.gov/22745249/) | **PMC全文**: [PMC6286148](https://pmc.ncbi.nlm.nih.gov/articles/PMC6286148/)

### 实验三：人类细胞基因组编辑（Cong et al., 2013 / Mali et al., 2013）

张锋团队和Church团队分别独立证明CRISPR-Cas9可在人类和小鼠细胞中对内源基因（如*EMX1*、*PNK*）进行精确切割和编辑。张锋团队还展示了多重编辑能力——同时切割多个基因位点。这实现了从体外到活细胞的关键跨越，使CRISPR真正成为可用的基因组编辑工具。

- **论文**: [Cong et al., 2013](https://pubmed.ncbi.nlm.nih.gov/23287718/) | [Mali et al., 2013](https://pubmed.ncbi.nlm.nih.gov/23287722/)

### 实验四：碱基编辑（Komor et al., 2016）

David Liu团队将Cas9 nickase（D10A，只切一条链）与大鼠胞嘧啶脱氨酶APOBEC1融合，创造出CBE。该系统在不产生双链断裂的情况下，将靶位点附近的胞嘧啶（C）直接脱氨为尿嘧啶（U），经复制修复后变为胸腺嘧啶（T），实现C→T转换。开创了"无断裂编辑"的新范式。

- **论文**: [Komor et al., 2016](https://pubmed.ncbi.nlm.nih.gov/27096365/)

### 实验五：引物编辑（Anzalone et al., 2019）

David Liu团队将Cas9(H840A) nickase与工程化逆转录酶融合，使用pegRNA作为向导。pegRNA不仅引导Cas9定位，其3'端延伸的逆转录模板（RTT）还编码所需编辑序列。Cas9切割非互补链后，释放的3'端作为引物被逆转录酶延伸，写入新序列。该系统在人细胞中完成了175种以上编辑，包括纠正镰刀型贫血（*HBB*）和Tay-Sachs病（*HEXA*）的致病突变。

- **论文**: [Anzalone et al., 2019](https://pubmed.ncbi.nlm.nih.gov/31634902/) | **PMC全文**: [PMC6907074](https://pmc.ncbi.nlm.nih.gov/articles/PMC6907074/)

---

## 📖 小故事

### 从酸奶到诺贝尔奖：CRISPR的意外起源

CRISPR的故事始于一个看似平凡的工业问题——如何让酸奶细菌抵抗噬菌体感染。

2002年，西班牙阿利坎特大学的Francisco Mojica在研究古菌和细菌的基因组时，注意到一组奇特的重复序列。他发现这些重复序列之间被间隔序列分开，而这些间隔序列与病毒DNA高度匹配。Mojica意识到，这些"间隔序列"本质上是细菌对过去病毒入侵的"记忆"——细菌将入侵病毒的DNA片段存储在CRISPR阵列中，以此识别并抵御未来的感染。他与Ruud Jansen共同将这一系统命名为"CRISPR"（Clustered Regularly Interspaced Short Palindromic Repeats）。

2007年，Danisco公司的Rodolphe Barrangou（当时在研究用于酸奶发酵的*Streptococcus thermophilus*）通过实验验证了Mojica的假说。他们发现，当细菌成功抵抗噬菌体感染后，其CRISPR阵列中新增了对应噬菌体的间隔序列。这一发现发表在*Science*上（[Barrangou et al., 2007](https://pubmed.ncbi.nlm.nih.gov/17379808/)），标志着CRISPR从"奇特的重复序列"转变为"被理解的免疫系统"。

此后，Charpentier发现了tracrRNA，Doudna与Charpentier合作将系统简化为可编程工具，张锋将其引入人类细胞——一条从酸奶发酵到诺贝尔奖的漫长道路，历时逾十年，跨越了基础研究与产业应用的鸿沟。

2012年的奠基论文发表后，CRISPR技术的传播速度前所未有——从论文发表到全球实验室广泛采用仅用了不到一年。2020年，Doudna和Charpentier因"开发基因组编辑方法"获得诺贝尔化学奖，这是科学史上首次由两位女性科学家独享诺贝尔科学奖项。

- **Wikipedia**: [Francisco Mojica](https://en.wikipedia.org/wiki/Francisco_Mojica)

---

## 🤔 思考题

1. **技术比较**：ZFN、TALEN和CRISPR-Cas9三种基因编辑技术各有何优缺点？为什么CRISPR能迅速取代前两者成为主流工具？请从可编程性、成本、效率和特异性四个维度分析。

2. **修复机制**：NHEJ和HDR两种DNA修复途径在基因编辑中的应用场景有何不同？如果你需要在一个基因中引入一个精确的点突变，你会选择哪种策略？为什么HDR在非分裂细胞中的效率很低？

3. **伦理边界**：2018年贺建奎"基因编辑婴儿"事件引发了全球震动。请讨论：体细胞编辑与生殖系编辑的核心伦理区别是什么？在什么条件下（如果有的话）生殖系基因编辑可以被接受？参考[贺建奎事件分析 (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC6431114/)和[He Jiankui (Wikipedia)](https://en.wikipedia.org/wiki/He_Jiankui)。

4. **临床转化**：2023年12月FDA批准的Casgevy（exa-cel）是全球首个CRISPR疗法。请分析其治疗镰刀型细胞贫血病的机制——为什么编辑*BCL11A*增强子可以治疗SCD？这种"自体细胞体外编辑再回输"的策略与直接体内编辑相比有何优势？参考[FDA批准综述 (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC11374260/)。

5. **前沿思考**：引物编辑理论上可纠正89%的致病变异，但当前效率仍低于CRISPR-Cas9。你认为阻碍引物编辑广泛应用的主要技术瓶颈是什么？未来5年内可能取得哪些突破？

6. **农业应用**：基因编辑作物与转基因作物在监管和公众接受度上有何不同？请以抗白粉病小麦为例，讨论基因编辑在作物育种中的优势与挑战。参考[作物保护综述 (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC12825932/)。

---

## 📖 术语表

| 术语 | 英文 | 释义 |
|------|------|------|
| CRISPR | Clustered Regularly Interspaced Short Palindromic Repeats | 规律间隔成簇短回文重复序列，细菌适应性免疫系统的组成部分 |
| Cas9 | CRISPR-associated protein 9 | CRISPR相关蛋白9，RNA引导的DNA核酸内切酶 |
| sgRNA | Single Guide RNA | 单链向导RNA，由crRNA和tracrRNA融合而成 |
| crRNA | CRISPR RNA | CRISPR RNA，含靶序列识别信息 |
| tracrRNA | trans-activating CRISPR RNA | 反式激活CRISPR RNA，辅助Cas9结合crRNA |
| PAM | Protospacer Adjacent Motif | 前间区序列邻近基序，Cas9识别靶DNA的必要序列（通常为NGG） |
| DSB | Double-Strand Break | 双链断裂，DNA两条链同时断裂 |
| NHEJ | Non-Homologous End Joining | 非同源末端连接，易出错的DNA修复途径 |
| HDR | Homology-Directed Repair | 同源定向修复，精确的DNA修复途径，需模板DNA |
| ZFN | Zinc Finger Nuclease | 锌指核酸酶，第一代可编程基因编辑工具 |
| TALEN | Transcription Activator-Like Effector Nuclease | 转录激活因子样效应物核酸酶，第二代基因编辑工具 |
| CBE | Cytosine Base Editor | 胞嘧啶碱基编辑器，将C转换为T |
| ABE | Adenine Base Editor | 腺嘌呤碱基编辑器，将A转换为G |
| pegRNA | Prime Editing Guide RNA | 引物编辑向导RNA，含PBS和RTT结构 |
| PBS | Primer Binding Site | 引物结合位点，pegRNA中与靶链3'端互补的序列 |
| RTT | Reverse Transcriptase Template | 逆转录模板，pegRNA中编码所需编辑的序列 |
| 脱靶效应 | Off-target Effect | 在非靶标位点产生的意外编辑 |
| 基因敲除 | Gene Knockout | 通过破坏基因功能使基因失活 |
| 基因敲入 | Gene Knock-in | 将外源序列精确插入基因组的特定位置 |
| Casgevy | exa-cel | 全球首个获批的CRISPR疗法，用于治疗镰刀型细胞贫血病 |

---

## 🔮 下节预告

### Day 89：CRISPR-Cas9系统

明天我们将深入探讨CRISPR-Cas9系统的分子细节：

- **Cas9蛋白的晶体结构与催化机制**：HNH和RuvC结构域如何协同切割DNA
- **sgRNA设计的优化策略**：on-target效率与off-target特异性的平衡
- **Cas9变体**：SpCas9、SaCas9、xCas9、高保真变体的比较
- **CRISPR-Cas系统的多样性**：Cas12、Cas13等新型系统的发现与应用
- **递送系统**：AAV、LNP等体内递送策略的进展与挑战

> 📌 **预习建议**：阅读[Doudna & Charpentier, Science, 2014综述](https://pubmed.ncbi.nlm.nih.gov/25299471/)，了解CRISPR-Cas9技术全景。

---

## 🔗 综合学习资源

### 权威机构资源
- [诺贝尔奖2020化学奖科学背景文档 (PDF)](https://www.nobelprize.org/uploads/2020/10/advanced-chemistryprize2020.pdf)
- [Broad Institute CRISPR问答](https://www.broadinstitute.org/what-broad/areas-focus/project-spotlight/questions-and-answers-about-crispr)
- [Doudna实验室出版物](https://doudnalab.org/publications/)
- [David Liu关键论文列表](https://www.liugroup.us/key-publications-2/)
- [NHGRI: Editing The Book Of Life With Molecular Scissors](https://www.genome.gov/editing-the-book-of-life-with-molecular-scissors)

### NCBI/PMC综述全文
- [Recent advances in therapeutic CRISPR-Cas9](https://pmc.ncbi.nlm.nih.gov/articles/PMC10080534/)
- [Advancing CRISPR genome editing into gene therapy clinical trials](https://pmc.ncbi.nlm.nih.gov/articles/PMC12094669/)
- [A CRISPR view of the 2020 Nobel Prize in Chemistry](https://pmc.ncbi.nlm.nih.gov/articles/PMC7773339/)
- [History of genome editing: From meganucleases to CRISPR](https://journals.sagepub.com/doi/pdf/10.1177/0023677221994613)

### 视频资源
- **B站**: [CRISPR-Cas9基因编辑技术基本概念及原理](https://www.bilibili.com/video/BV1Pmm5BeE68/) | [Cas9 RNP基因编辑实操](https://www.bilibili.com/video/BV1DajU6YENJ/)
- **YouTube**: [Jennifer Doudna讲解CRISPR](https://www.youtube.com/watch?v=SuAxDVBt7kQ) | [CRISPR-Cas9动画演示](https://www.youtube.com/watch?v=2pp7E5-X1Ek)

### GitHub仓库
- **学习资源仓库**: [genetics-learning-100-days](https://github.com/lijianguoa/genetics-learning-100-days)
- **图片资源仓库**: [genetics-images](https://github.com/lijianguoa/genetics-images)



---

## 📎 补充学习资源链接

> 以下资源由workflow.py自动检测并补充。

### Cas9

- [Wikipedia(英)](https://en.wikipedia.org/wiki/Cas9)

### 基因编辑

- [Wikipedia(英)](https://en.wikipedia.org/wiki/Gene_editing)

### 贺建奎

- [Wikipedia(中)](https://zh.wikipedia.org/wiki/贺建奎)

---

*本内容由遗传学100天学习计划自动生成 | Day 88/100 | 2026-08-10*
