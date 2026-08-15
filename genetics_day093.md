# 遗传学100天学习计划 · Day 93

# 生物信息学与遗传学

> **系列**: 遗传学100天学习计划 | **部分**: 第七部分 现代遗传学（第81-95天）
> **日期**: 2026年8月15日 | **Day**: 093/100
> **主题**: Bioinformatics and Genetics — 生物信息学如何重塑遗传学研究

---

## 一、配图

### 配图1：生物信息学与遗传学交汇
![生物信息学与遗传学](genetics_day093_img1.jpg)

*DNA双螺旋与计算数据的融合——生物信息学的核心隐喻。左为经典遗传学（DNA结构），右为计算分析（序列比对、二进制数据流），中央是序列比对可视化。*

### 配图2：BLAST算法工作流程
![BLAST算法流程](genetics_day093_img2.jpg)

*BLAST算法的完整工作流程：序列输入 → 字匹配 → 数据库扫描 → HSP延伸 → 统计评估 → 结果输出。这是生物信息学中最广泛使用的算法之一。*

---

## 二、历史背景

### 从手工分析到计算革命

生物信息学的历史可以追溯到20世纪60年代，比DNA测序技术的出现还要早。其根基建立在将计算方法应用于**蛋白质序列分析**之上。

**关键时间线：**

| 年份 | 里程碑事件 |
|------|-----------|
| 1955 | Frederick Sanger 测定首个蛋白质（胰岛素）的完整氨基酸序列 |
| 1960 | Margaret Dayhoff 开发 **COMPROTEIN**——世界上第一个生物信息学软件 |
| 1965 | Dayhoff 出版 **《Atlas of Protein Sequence and Structure》**——第一个生物序列数据库，仅含65个蛋白质序列 |
| 1970 | Needleman 和 Wunsch 发表全局序列比对算法 |
| 1974 | Dayhoff 发表 **PAM矩阵**——第一个氨基酸替换概率模型 |
| 1978 | Paulien Hogeweg 首次使用"bioinformatics"一词 |
| 1981 | Smith 和 Waterman 发表局部序列比对算法 |
| 1982 | **GenBank** 建立；EMBL核苷酸序列数据库同年起源 |
| 1988 | **NCBI**（美国国家生物技术信息中心）正式成立 |
| 1990 | Altschul 等人发表 **BLAST** 算法 |
| 1994 | Thompson 等人发表 **ClustalW** |
| 1999 | **Ensembl** 基因组浏览器建立 |
| 2003 | 人类基因组计划完成 |
| 2005 | 第一篇成功的 **GWAS** 论文发表 |

> 📖 **延伸阅读**: [A brief history of bioinformatics](https://academic.oup.com/bib/article/20/6/1981/5260796) (Gauthier et al., 2019, *Briefings in Bioinformatics*)
> 📖 **延伸阅读**: [The origins of bioinformatics](https://www.nature.com/articles/35042090) (Hagen, 2000, *Nature Reviews Genetics*)

### 三大数据库的建立

生物信息学的发展离不开数据共享的国际合作。1988年，三大核苷酸序列数据库——美国的 [GenBank](https://www.ncbi.nlm.nih.gov/genbank/)（NCBI）、欧洲的 [ENA](https://www.ebi.ac.uk/ena/browser/home)（EMBL-EBI）和日本的 [DDBJ](https://www.ddbj.nig.ac.jp/)——启动了**国际核苷酸序列数据库合作组织（INSDC）**，每日交换数据，形成了全球统一的序列数据网络。

> 🔗 [Wikipedia: Bioinformatics](https://en.wikipedia.org/wiki/Bioinformatics)
> 🔗 [Wikipedia: NCBI](https://en.wikipedia.org/wiki/National_Center_for_Biotechnology_Information)
> 🔗 [Wikipedia: EMBL-EBI](https://en.wikipedia.org/wiki/European_Bioinformatics_Institute)

---

## 三、核心概念

### 3.1 序列比对（Sequence Alignment）

序列比对是生物信息学最基础的操作，用于比较两条或多条生物序列（DNA、RNA或蛋白质）之间的相似性。

- **全局比对**：[Needleman-Wunsch算法](https://en.wikipedia.org/wiki/Needleman-Wunsch_algorithm)（1970），基于动态规划，对两条序列进行端到端的完整比对，时间复杂度 O(mn)
- **局部比对**：[Smith-Waterman算法](https://en.wikipedia.org/wiki/Smith-Waterman_algorithm)（1981），找出两条序列中相似度最高的局部片段
- **多序列比对**：同时比对三条以上序列，用于揭示保守区域和进化关系。代表方法包括渐进式比对（[ClustalW](https://en.wikipedia.org/wiki/Clustal)）、迭代比对（MUSCLE、MAFFT）

> 🎥 **B站视频**: [北京大学生物信息学课程——序列数据库与BLAST算法](https://www.bilibili.com/video/BV13t411G7oh)
> 🎥 **B站视频**: [十分钟吃透BLAST比对底层逻辑并实操](https://www.bilibili.com/opus/907822989664321544)

### 3.2 基因组组装（Genome Assembly）

基因组组装是将测序产生的短片段（reads）拼接成完整基因组序列的过程：

- **OLC策略**（重叠-共识-拼接）：用于第一代测序数据
- **De Bruijn图**方法：广泛应用于下一代测序（NGS）数据，如 SPAdes、Velvet 等组装器
- 组装结果由 **contig**（连续序列）→ **scaffold**（支架）→ **染色体级别组装**逐步提升

### 3.3 基因组注释（Genome Annotation）

基因组注释是指在基因组序列上识别和标注功能元件的过程：

- **基因预测**：识别编码基因的位置（如 GeneMark、AUGUSTUS）
- **功能注释**：通过数据库比对推断基因功能
- **结构注释**：识别外显子、内含子、UTR、调控元件等

[Ensembl](https://en.wikipedia.org/wiki/Ensembl_genome_browser) 项目就是自动注释工具的代表，2000年5月已确认人类基因组上超过35,000个基因的位置。

### 3.4 变异检测与GWAS

- **变异检测**：从测序数据中识别SNP、Indel、结构变异（SV）和拷贝数变异（CNV）
- **GWAS（全基因组关联研究）**：在全基因组范围内扫描大量SNP，寻找与特定性状或疾病相关的遗传变异
- 主要工具：[GATK](https://gatk.broadinstitute.org/)、DeepVariant、PLINK

> 🔗 [Wikipedia: Genome-wide association study](https://en.wikipedia.org/wiki/Genome-wide_association_study)
> 🔗 [GWAS Catalog (NHGRI-EBI)](https://www.ebi.ac.uk/gwas/)

### 3.5 生物信息学数据库生态

| 数据库 | 机构 | 主要内容 | 链接 |
|--------|------|---------|------|
| GenBank | NCBI (美国) | 核苷酸序列 | [ncbi.nlm.nih.gov/genbank](https://www.ncbi.nlm.nih.gov/genbank/) |
| ENA | EMBL-EBI (欧洲) | 核苷酸序列 | [ebi.ac.uk/ena](https://www.ebi.ac.uk/ena/browser/home) |
| DDBJ | NIG (日本) | 核苷酸序列 | [ddbj.nig.ac.jp](https://www.ddbj.nig.ac.jp/) |
| UniProt | EBI/SIB (联合) | 蛋白质序列与功能 | [uniprot.org](https://www.uniprot.org/) |
| Ensembl | EBI/Sanger (联合) | 基因组浏览器 | [ensembl.org](https://www.ensembl.org/) |
| dbSNP | NCBI | SNP数据库 | [ncbi.nlm.nih.gov/snp](https://www.ncbi.nlm.nih.gov/snp/) |

---

## 四、科学家故事

### 4.1 Margaret Dayhoff（1925-1983）——生物信息学之母

Margaret Dayhoff 被NCBI前主任David Lipman称为"生物信息学之母之父"。她的贡献堪称奠基性：

- 1960年开发 **COMPROTEIN**——世界上第一个生物信息学软件，用FORTRAN编写于IBM 7090上运行
- 1965年出版 **《Atlas of Protein Sequence and Structure》**——第一个生物序列数据库
- 发明了至今仍在使用的**单字母氨基酸代码**
- 1974年发表 **PAM矩阵**——第一个氨基酸替换概率模型

Dayhoff在量子化学和蛋白质化学的交叉领域工作，她的远见卓识为整个生物信息学领域奠定了基础。

> 🔗 [Wikipedia: Margaret Oakley Dayhoff](https://en.wikipedia.org/wiki/Margaret_Oakley_Dayhoff)

### 4.2 David J. Lipman ——NCBI的掌舵人

David J. Lipman 自1989年起担任美国国家生物技术信息中心（NCBI）主任。他是 **BLAST** 序列比对程序和 **FASTA** 算法的原始作者之一。

在Lipman的领导下，NCBI从最初仅8名工作人员发展为拥有500多人的分子生物学信息枢纽。他领导开发了PubMed、GenBank、Entrez等核心资源，彻底改变了全球生物学家的数据获取方式。他曾获得三枚公共卫生服务杰出服务奖章和多项国家级奖项。

> 🔗 [NCBI历史: A Brief History of NCBI's Formation and Growth](https://www.ncbi.nlm.nih.gov/books/NBK148949/)

### 4.3 Temple F. Smith & Michael S. Waterman ——局部比对算法之父

1981年，Temple F. Smith和Michael S. Waterman共同发表了**Smith-Waterman局部比对算法**，这是序列比对领域的里程碑。

Smith曾在北密歇根大学物理系担任教授，后转至波士顿大学生物医学工程系。Waterman是南加州大学教授，除了Smith-Waterman算法外，他还对序列组装理论（Lander-Waterman模型）做出了重大贡献。

> 🔗 [Wikipedia: Temple F. Smith](https://en.wikipedia.org/wiki/Temple_F._Smith)
> 🔗 [Smith-Waterman 1981原文PDF](https://computingbiology.github.io/docs/smithwaterman1981.pdf)

### 4.4 Eugene V. Koonin ——进化基因组学先驱

Eugene V. Koonin 是NCBI进化基因组学小组的领导者，美国国家科学院院士。他于1991年加入NCBI，主要贡献包括：

- 开发了**直系同源基因簇（COGs）**概念——基因组功能和进化分析的核心框架
- 对 **CRISPR-Cas系统**的开创性研究：2005年假设CRISPR间隔DNA可能是适应性免疫系统的一部分，这一假说后来成为CRISPR基因编辑技术的基础
- 对几乎所有细胞生物学特征进行了比较基因组学分析

> 🔗 [Wikipedia: Eugene Koonin](https://en.wikipedia.org/wiki/Eugene_Koonin)
> 🔗 [PNAS: Profile of Eugene V. Koonin](https://www.pnas.org/doi/pdf/10.1073/pnas.1621406114)

### 4.5 Michael Gribskov ——Profile分析方法

Michael Gribskov 开发了**Profile分析方法**——利用位置特异性评分矩阵（PSSM）检测蛋白质序列中远缘相似性的方法。这一方法后来影响了PSI-BLAST和隐马尔可夫模型（HMMER）的发展。

> 代表论文: Gribskov, M., McLachlan, A.D., & Eisenberg, D. (1987). "Profile analysis: detection of distantly related proteins." *PNAS*, 84(13), 4355-4358.

---

## 五、重要文献

### 5.1 BLAST（1990）——被引用最多的科学论文之一

> Altschul, S.F., Gish, W., Miller, W., Myers, E.W., & Lipman, D.J. (1990). "Basic local alignment search tool." *Journal of Molecular Biology*, 215(3), 403-410.

- **DOI**: [10.1016/S0022-2836(05)80360-2](https://doi.org/10.1016/S0022-2836(05)80360-2)
- **NCBI**: [PubMed 2231712](https://pubmed.ncbi.nlm.nih.gov/2231712/)
- 这篇论文是1990年代被引用次数最多的科学论文之一，原始论文已被引用超过50,000次
- 🔗 [BLAST官网](https://blast.ncbi.nlm.nih.gov/Blast.cgi)

### 5.2 Gapped BLAST & PSI-BLAST（1997）

> Altschul, S.F., Madden, T.L., Schäffer, A.A., Zhang, J., Zhang, Z., Miller, W., & Lipman, D.J. (1997). "Gapped BLAST and PSI-BLAST: a new generation of protein database search programs." *Nucleic Acids Research*, 25(17), 3389-3402.

- **DOI**: [10.1093/nar/25.17.3389](https://doi.org/10.1093/nar/25.17.3389)
- **PMC**: [PMC146917](https://pmc.ncbi.nlm.nih.gov/articles/PMC146917/)

### 5.3 FASTA（1988）

> Pearson, W.R. & Lipman, D.J. (1988). "Improved tools for biological sequence comparison." *PNAS*, 85(8), 2444-2448.

- **DOI**: [10.1073/pnas.85.8.2444](https://doi.org/10.1073/pnas.85.8.2444)
- **PNAS原文**: [pnas.org/lookup/doi/10.1073/pnas.85.8.2444](https://www.pnas.org/lookup/doi/10.1073/pnas.85.8.2444)

### 5.4 Smith-Waterman（1981）

> Smith, T.F. & Waterman, M.S. (1981). "Identification of common molecular subsequences." *Journal of Molecular Biology*, 147(1), 195-197.

- **DOI**: [10.1016/0022-2836(81)90087-5](https://doi.org/10.1016/0022-2836(81)90087-5)
- **原文PDF**: [Smith-Waterman 1981](https://computingbiology.github.io/docs/smithwaterman1981.pdf)

### 5.5 ClustalW（1994）

> Thompson, J.D., Higgins, D.G., & Gibson, T.J. (1994). "CLUSTAL W: improving the sensitivity of progressive multiple sequence alignment through sequence weighting, position-specific gap penalties and weight matrix choice." *Nucleic Acids Research*, 22(22), 4673-4680.

- **DOI**: [10.1093/nar/22.22.4673](https://doi.org/10.1093/nar/22.22.4673)
- **PMC**: [PMC308517](https://pmc.ncbi.nlm.nih.gov/articles/PMC308517/)

### 5.6 第一篇GWAS论文（2005）

> Klein, R.J., Zeiss, C., Chew, E.Y., Tsai, J.Y., Sackler, R.S., Haynes, C., et al. (2005). "Complement Factor H polymorphism in age-related macular degeneration." *Science*, 308(5720), 385-389.

- **DOI**: [10.1126/science.1109557](https://doi.org/10.1126/science.1109557)
- 在96个病例和50个对照中检测了116,204个SNP，发现了CFH基因变异与AMD的强关联

### 5.7 生物信息学简史综述（2019）

> Gauthier, J., Vincent, A.T., Charette, S.J., & Derome, N. (2019). "A brief history of bioinformatics." *Briefings in Bioinformatics*, 20(6), 1981-1996.

- **DOI**: [10.1093/bib/bby063](https://doi.org/10.1093/bib/bby063)
- **PDF**: [academic.oup.com](https://academic.oup.com/bib/article-pdf/20/6/1981/31789310/bby063.pdf)

---

## 六、经典实验与工具

### 6.1 BLAST——最广泛使用的序列搜索工具

**开发者**: Stephen Altschul, Warren Gish, Webb Miller, Eugene Myers, David Lipman（1990）

**核心原理**：通过"字"（word）匹配→延伸策略，快速寻找局部相似性。包含五个关键步骤：

1. **过滤**（Filtering）：移除低复杂度区域
2. **种子**（Seeding）：生成短字列表
3. **数据库扫描**：在数据库中寻找字匹配
4. **HSP延伸**：向两端延伸高得分片段对
5. **显著性分析**：计算E值评估统计显著性

> 🔗 [BLAST官网](https://blast.ncbi.nlm.nih.gov/Blast.cgi) | [Wikipedia: BLAST](https://en.wikipedia.org/wiki/BLAST_(biotechnology))

### 6.2 FASTA——BLAST的前辈

**开发者**: William R. Pearson & David J. Lipman（1988）

**原理**: 使用k-tuple（短匹配词）快速识别序列间的相似区域，然后进行更精细的比对。FASTA是BLAST之前的主要工具，至今仍在使用。

> 🔗 [Wikipedia: FASTA](https://en.wikipedia.org/wiki/FASTA)

### 6.3 ClustalW——多序列比对的标准

**开发者**: Julie D. Thompson, Desmond G. Higgins, Toby J. Gibson（1994）

**原理**: 渐进式多序列比对——先计算两两距离，构建引导树，然后沿引导树逐步添加序列进行比对。原始版Clustal由Des Higgins于1988年创建。

> 🔗 [Wikipedia: Clustal](https://en.wikipedia.org/wiki/Clustal)

### 6.4 全基因组测序分析流程

现代WGS分析的标准流程：

```
原始数据 → FastQC质量控制 → BWA/Bowtie2序列比对 → 
BQSR质量校准 → GATK/DeepVariant变异检测 → 
VEP/ANNOVAR变异注释 → 下游分析
```

### 6.5 GWAS分析流程

```
基因型数据 → 质量控制 → 基因型插值(Imputation) → 
关联分析(PLINK) → 多重检验校正 → 曼哈顿图 → 
功能注释与验证
```

> 🎥 **B站视频**: [山东大学生物信息学课程（全套课件）](https://www.bilibili.com/opus/1062293520003366930)

---

## 七、小故事

### 故事一：Margaret Dayhoff与单字母氨基酸代码

1960年代，当大多数科学家还在用三字母缩写（如Ala、Gly、Val）表示氨基酸时，Margaret Dayhoff意识到随着序列数据的增长，需要更紧凑的表示方式。她发明了**单字母氨基酸代码**——用A代表丙氨酸、G代表甘氨酸、V代表缬氨酸等。这套编码系统如此简洁高效，以至于半个多世纪后的今天，全世界每一个生物信息学软件、每一个蛋白质数据库仍在使用它。

有趣的是，有些字母的分配并非取首字母——例如赖氨酸用K（而非L，因为L已分配给亮氨酸），色氨酸用W（因为T已分配给苏氨酸）。这些"妥协"恰恰反映了Dayhoff在设计时的全局思考。

### 故事二：BLAST的诞生

1990年，Stephen Altschul和David Lipman在NCBI发表BLAST算法时，可能没有预料到它将成为生物学历史上被引用最多的论文之一。在BLAST之前，序列搜索主要依赖FASTA和Smith-Waterman算法。Smith-Waterman虽然精确，但速度太慢，无法应对快速增长的大型数据库。

BLAST的巧妙之处在于：它通过"字"匹配策略大幅缩小搜索空间，同时利用严格的统计学方法（Karlin-Altschul统计学）评估匹配的显著性。这种"快而准"的设计理念使BLAST成为生物信息学的标志性工具。据说，BLAST论文发表后不久，NCBI的服务器就因为全球科学家的查询请求而几乎瘫痪。

### 故事三：Koonin与CRISPR的预言

2005年，Eugene Koonin在NCBI进行比较基因组学分析时注意到一个奇特现象：细菌和古菌的CRISPR位点中的"间隔DNA"（spacer DNA）序列，与噬菌体基因组序列高度匹配。他大胆假设这可能是一种未知的**适应性免疫系统**——细菌通过存储入侵噬菌体的DNA片段来"记住"敌人，从而在再次遇到相同噬菌体时进行防御。

这一假设在当时极具争议性，但后来被实验完全证实，并直接催生了CRISPR-Cas9基因编辑技术。Koonin的故事展示了生物信息学比较分析的预见性力量——纯计算分析可以揭示实验生物学尚未发现的生物学机制。

---

## 八、思考题

1. **算法比较**：Smith-Waterman算法保证找到最优局部比对，但时间复杂度为O(mn)；BLAST通过启发式策略大幅提升速度但可能遗漏某些匹配。在实际研究中，如何权衡精度与速度？在什么场景下必须使用Smith-Waterman而非BLAST？

2. **数据库伦理**：GenBank等公共数据库实现了全球序列数据的免费共享。但这种开放共享是否带来了伦理挑战？例如，人类基因组数据可能泄露个人隐私信息，如何平衡开放科学与数据保护？

3. **GWAS的局限性**：第一篇GWAS论文（Klein et al., 2005）仅用96个病例和50个对照就发现了CFH基因与AMD的关联。然而，现代GWAS通常需要数万样本。为什么GWAS对样本量的需求急剧增长？这反映了遗传学研究的什么本质特征？

4. **从序列到功能**：生物信息学工具可以快速比对序列、预测基因位置，但"序列相似"是否等同于"功能相似"？在什么情况下同源基因可能具有截然不同的功能？

5. **未来展望**：随着深度学习在生物信息学中的应用（如AlphaFold预测蛋白质结构、DeepVariant进行变异检测），传统算法（如BLAST、Smith-Waterman）是否会被完全取代？还是两者会长期共存、互补使用？

6. **Dayhoff的遗产**：Margaret Dayhoff在1960年代就预见到了序列数据爆炸的必要性，并为此建立了数据库和编码系统。如果她活到今天，会对生物信息学的哪些发展感到惊讶？哪些发展可能超出了她的预期？

---

## 九、术语表

| 术语 | 英文 | 释义 |
|------|------|------|
| 生物信息学 | Bioinformatics | 利用计算方法分析生物数据的交叉学科 |
| 序列比对 | Sequence Alignment | 比较两条或多条生物序列相似性的方法 |
| 全局比对 | Global Alignment | 对两条序列进行端到端的完整比对 |
| 局部比对 | Local Alignment | 找出两条序列中相似度最高的局部片段 |
| 动态规划 | Dynamic Programming | 一种通过子问题最优解构建整体最优解的算法策略 |
| 多序列比对 | Multiple Sequence Alignment (MSA) | 同时比对三条以上序列的方法 |
| 基因组组装 | Genome Assembly | 将测序短片段拼接成完整基因组序列的过程 |
| 基因组注释 | Genome Annotation | 在基因组序列上识别和标注功能元件 |
| 变异检测 | Variant Calling | 从测序数据中识别基因组变异 |
| 全基因组关联研究 | GWAS (Genome-Wide Association Study) | 全基因组范围内扫描SNP与性状的关联 |
| 单核苷酸多态性 | SNP (Single Nucleotide Polymorphism) | 基因组中单个碱基的变异 |
| PAM矩阵 | PAM Matrix | Point Accepted Mutation，氨基酸替换概率模型 |
| E值 | E-value | BLAST中评估匹配统计显著性的期望值 |
| 直系同源 | Orthology | 不同物种中由共同祖先基因分化而来的同源基因 |
| 旁系同源 | Paralogy | 同一基因组内因复制事件产生的同源基因 |
| 基因型插值 | Genotype Imputation | 基于参考面板推测未直接基因分型的SNP |
| 位置特异性评分矩阵 | PSSM (Position-Specific Scoring Matrix) | Profile分析中用于检测远缘相似性的矩阵 |
| 隐马尔可夫模型 | HMM (Hidden Markov Model) | 用于序列 profile 分析的概率模型 |
| De Bruijn图 | De Bruijn Graph | 基因组组装中基于k-mer的图结构 |
| 参考基因组 | Reference Genome | 作为比对和变异检测标准的基因组序列 |

---

## 十、下节预告

### Day 94：精准医学

明天我们将探讨**精准医学（Precision Medicine）**——生物信息学与遗传学的终极应用。

精准医学旨在根据个体的基因组信息，为其量身定制疾病预防和治疗方案。从肿瘤基因组学分型到药物基因组学，从遗传病筛查到个性化癌症免疫治疗，精准医学正在将遗传学从实验室推向临床。

我们将讨论：
- 精准医学的概念与发展历程
- 肿瘤精准医学与伴随诊断
- 药物基因组学与个体化用药
- 多组学数据整合在精准医学中的应用
- 精准医学的伦理、法律与社会影响
- 中国精准医学计划与美国Precision Medicine Initiative

> 💡 **预习建议**: 了解 [All of Us Research Program](https://allofus.nih.gov/) 和 [中国精准医学计划](https://en.wikipedia.org/wiki/Precision_medicine) 的基本框架

---

## 参考资源汇总

### 在线工具与数据库
- [NCBI BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi) — 序列搜索工具
- [NCBI GenBank](https://www.ncbi.nlm.nih.gov/genbank/) — 核苷酸序列数据库
- [Ensembl](https://www.ensembl.org/) — 基因组浏览器
- [UniProt](https://www.uniprot.org/) — 蛋白质数据库
- [GWAS Catalog](https://www.ebi.ac.uk/gwas/) — GWAS目录
- [GATK](https://gatk.broadinstitute.org/) — 基因组分析工具包

### Wikipedia链接
- [Bioinformatics](https://en.wikipedia.org/wiki/Bioinformatics)
- [BLAST](https://en.wikipedia.org/wiki/BLAST_(biotechnology))
- [Smith-Waterman algorithm](https://en.wikipedia.org/wiki/Smith-Waterman_algorithm)
- [FASTA](https://en.wikipedia.org/wiki/FASTA)
- [Clustal](https://en.wikipedia.org/wiki/Clustal)
- [GenBank](https://en.wikipedia.org/wiki/GenBank)
- [NCBI](https://en.wikipedia.org/wiki/National_Center_for_Biotechnology_Information)
- [EMBL-EBI](https://en.wikipedia.org/wiki/European_Bioinformatics_Institute)
- [Ensembl](https://en.wikipedia.org/wiki/Ensembl_genome_browser_project)
- [GWAS](https://en.wikipedia.org/wiki/Genome-wide_association_study)
- [Margaret Dayhoff](https://en.wikipedia.org/wiki/Margaret_Oakley_Dayhoff)
- [Eugene Koonin](https://en.wikipedia.org/wiki/Eugene_Koonin)
- [Temple F. Smith](https://en.wikipedia.org/wiki/Temple_F._Smith)
- [Needleman-Wunsch algorithm](https://en.wikipedia.org/wiki/Needleman-Wunsch_algorithm)

### 视频资源
- 🎥 [北京大学生物信息学课程](https://www.bilibili.com/video/BV13t411G7oh) (B站)
- 🎥 [山东大学生物信息学课程](https://www.bilibili.com/opus/1062293520003366930) (B站)
- 🎥 [十分钟吃透BLAST比对底层逻辑](https://www.bilibili.com/opus/907822989664321544) (B站)
- 🎥 [Sequence Alignment (YouTube)](https://www.classcentral.com/course/youtube-sequence-alignment-97525)

### NCBI文献链接
- [BLAST原文 (PubMed 2231712)](https://pubmed.ncbi.nlm.nih.gov/2231712/)
- [Gapped BLAST (PMC 146917)](https://pmc.ncbi.nlm.nih.gov/articles/PMC146917/)
- [ClustalW (PMC 308517)](https://pmc.ncbi.nlm.nih.gov/articles/PMC308517/)
- [NCBI历史](https://www.ncbi.nlm.nih.gov/books/NBK148949/)

---

*遗传学100天学习计划 · Day 93 · 2026年8月15日*
*下一期：Day 94 — 精准医学*
