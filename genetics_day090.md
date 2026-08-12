# Day 90：基因治疗的进展

> **遗传学100天学习计划** | Day 90 / 100  
> **主题**：[基因治疗](https://zh.wikipedia.org/wiki/基因治疗)的进展 — 从概念验证到临床现实的六十年征程  
> **日期**：2026年8月12日  
> **模块**：第七部分 · 现代遗传学（Day 81-95）

---

## 一、今日配图

![基因治疗机制示意图](./genetics_day090_img1.jpg)

*图1：[AAV](https://zh.wikipedia.org/wiki/腺相关病毒)载体介导的[基因治疗](https://zh.wikipedia.org/wiki/基因治疗)机制示意 — 从载体工程到细胞内递送再到蛋白表达的全过程*

![基因治疗发展时间线](./genetics_day090_img2.jpg)

*图2：基因治疗六十年发展里程碑（1990-2026）*

---

## 二、历史背景

基因治疗的构想可以追溯到20世纪60年代。1963年，美国分子生物学家乔舒亚·莱德伯格首次提出"通过外源DNA纠正人类遗传缺陷"的设想。1972年，西奥多·弗里德曼和理查德·罗布林在《科学》杂志上发表了具有里程碑意义的论文，正式提出了基因治疗的概念框架，呼吁科学界严肃对待这一可能"从根本上治疗遗传病"的新思路。

然而，真正的突破需要等待重组DNA技术的成熟。1980年代，[逆转录病毒载体](https://en.wikipedia.org/wiki/Retroviral_vector)技术的发展为基因治疗提供了关键的工具——科学家们学会将治疗基因装入改造过的病毒"快递盒"中，使其能高效进入人体细胞。

1990年9月14日，历史性的一刻到来。美国国立卫生研究院（NIH）的[威廉·弗伦奇·安德森](https://en.wikipedia.org/wiki/W._French_Anderson)团队完成了人类历史上第一例基因治疗临床试验。接受治疗的是一名4岁的[ADA-SCID](https://en.wikipedia.org/wiki/Adenosine_deaminase_deficiency)（腺苷脱氨酶缺陷重症联合免疫缺陷）患儿阿珊蒂·德席尔瓦。医生从她体内提取T细胞，用[逆转录病毒载体](https://en.wikipedia.org/wiki/Retroviral_vector)导入正常的ADA基因，再回输到她体内。治疗取得了令人振奋的效果——她的免疫系统功能得到了显著改善。

但基因治疗的道路并非坦途。1999年，18岁的[杰西·格尔辛格](https://en.wikipedia.org/wiki/Jesse_Gelsinger)在接受[腺病毒](https://zh.wikipedia.org/wiki/腺病毒)载体基因治疗后因严重的免疫反应不幸去世。这一悲剧震动了整个科学界，导致基因治疗临床试验大面积暂停，许多研究计划被迫搁置。格尔辛格之死深刻揭示了基因治疗安全性问题的严峻性，也推动了更严格的监管审查和载体安全性改进。

经过数十年的技术积累和教训反思，基因治疗在2010年代迎来了真正的复兴。2012年，欧洲药品管理局批准了全球首个基因治疗药物[Glybera](https://en.wikipedia.org/wiki/Alipogene_tiparvovec)（用于治疗脂蛋白脂肪酶缺乏症），标志着基因治疗从实验走向临床的现实转化。此后，[Luxturna](https://en.wikipedia.org/wiki/Voretigene_neparvovec)（2017）、[Zolgensma](https://en.wikipedia.org/wiki/Onasemnogene_abeparvovec)（2019）、[Casgevy](https://www.fda.gov/news-events/press-announcements/fda-approves-first-gene-therapy-young-children-sickle-cell-disease)（2023）等一系列里程碑式的基因治疗药物相继获批，基因治疗正式进入了临床应用的黄金时代。

---

## 三、核心概念

### 3.1 基因治疗的定义与分类

基因治疗是指通过将遗传物质导入患者细胞来治疗或预防疾病的技术。根据策略不同，基因治疗可分为以下几类：

**[基因增强](https://en.wikipedia.org/wiki/Gene_therapy#Gene_augmentation)（Gene Augmentation）**：向细胞导入一个功能正常的基因拷贝，以补偿缺陷基因的功能缺失。这是目前最成熟的策略，适用于隐性遗传病。[Luxturna](https://en.wikipedia.org/wiki/Voretigene_neparvovec)、[Zolgensma](https://en.wikipedia.org/wiki/Onasemnogene_abeparvovec)等获批药物均采用此策略。

**[基因编辑](https://zh.wikipedia.org/wiki/基因编辑)（Gene Editing）**：利用[CRISPR-Cas9](https://zh.wikipedia.org/wiki/[CRISPR](https://zh.wikipedia.org/wiki/CRISPR))等工具直接在基因组层面进行精确修改——可以敲除致病基因、纠正点突变或插入正常序列。[Casgevy](https://www.fda.gov/news-events/press-announcements/fda-approves-first-gene-therapy-young-children-sickle-cell-disease)是首个基于[CRISPR](https://zh.wikipedia.org/wiki/CRISPR)的获批基因治疗药物。

**[基因沉默](https://zh.wikipedia.org/wiki/基因沉默)（Gene Silencing）**：通过[RNA干扰](https://zh.wikipedia.org/wiki/RNA干扰)或[反义寡核苷酸](https://zh.wikipedia.org/wiki/反义寡核苷酸)技术抑制有害基因的表达，适用于显性遗传病或由有毒蛋白引起的疾病。

### 3.2 ex vivo 与 in vivo 两种递送策略

基因治疗的递送方式分为两大类：

**[ex vivo](https://en.wikipedia.org/wiki/Gene_therapy#Ex_vivo)（体外）策略**：从患者体内取出细胞（通常是[造血干细胞](https://zh.wikipedia.org/wiki/造血幹細胞)或T细胞），在实验室中进行基因改造，然后再回输到患者体内。Casgevy和[CAR-T](https://zh.wikipedia.org/wiki/CAR-T细胞)细胞疗法均采用此策略。优势是可以在体外精确控制[基因编辑](https://zh.wikipedia.org/wiki/基因编辑)效率，并进行质量检测；局限是流程复杂、成本高昂，且需要清淋预处理。

**[in vivo](https://en.wikipedia.org/wiki/Gene_therapy#In_vivo)（体内）策略**：将携带治疗基因的载体直接注射到患者体内，载体自行寻找到靶细胞并释放基因。[AAV](https://zh.wikipedia.org/wiki/腺相关病毒)载体是目前[in vivo](https://en.wikipedia.org/wiki/Gene_therapy#In_vivo)递送的主力军，Luxturna通过视网膜下注射、Zolgensma通过静脉注射给药。优势是操作简便、适用面广；挑战在于如何实现组织特异性靶向和避免免疫反应。

### 3.3 病毒载体系统

病毒载体是基因治疗最核心的递送工具，经过改造的病毒去除了致病基因，保留了高效感染和基因递送能力：

| 载体类型 | 包装容量 | 特点 | 代表药物 |
|----------|----------|------|----------|
| AAV（[腺相关病毒](https://zh.wikipedia.org/wiki/腺相关病毒)） | ~4.7 kb | [免疫原性](https://zh.wikipedia.org/wiki/免疫原性)低、长期表达、组织嗜性多样 | Luxturna, Zolgensma, [Elevidys](https://en.wikipedia.org/wiki/Delandistrogene_moxeparvovec) |
| 慢病毒 | ~8 kb | 可感染分裂与非分裂细胞、整合到基因组 | [CAR-T](https://zh.wikipedia.org/wiki/CAR-T细胞)疗法 |
| 逆转录病毒 | ~8 kb | 仅感染分裂细胞、整合到基因组 | 早期SCID基因治疗 |
| [腺病毒](https://zh.wikipedia.org/wiki/腺病毒) | ~36 kb | 高滴度、不整合、瞬时表达 | 早期试验（已少用） |

### 3.4 非病毒载体与新兴技术

近年来，非病毒递送系统快速发展。[脂质纳米颗粒](https://zh.wikipedia.org/wiki/脂质纳米颗粒)（[LNP](https://en.wikipedia.org/wiki/Lipid_nanoparticle)）因在mRNA疫苗中的成功应用而备受关注，正被探索用于基因治疗递送。[LNP](https://en.wikipedia.org/wiki/Lipid_nanoparticle)的优势在于可重复给药、规模化生产和较低的[免疫原性](https://zh.wikipedia.org/wiki/免疫原性)，但递送效率和靶向特异性仍需提升。

在基因编辑工具方面，[碱基编辑](https://en.wikipedia.org/wiki/Base_editing)和[先导编辑](https://en.wikipedia.org/wiki/Prime_editing)作为[CRISPR-Cas9](https://zh.wikipedia.org/wiki/CRISPR)的升级版本正在快速推进。[碱基编辑](https://en.wikipedia.org/wiki/Base_editing)可以在不产生DNA双链断裂的情况下实现单碱基转换，降低了脱靶风险；[先导编辑](https://en.wikipedia.org/wiki/Prime_editing)则能实现所有12种碱基替换以及小片段插入和缺失，被称为"搜索-替换"式基因编辑。截至2025年12月，全球已有136项CRISPR临床试验正在进行，其中36项基于体内递送，非病毒载体的使用比例显著上升。

---

## 四、科学家故事

### 詹妮弗·杜德纳与艾曼纽·卡彭蒂耶：CRISPR的发现者

2012年，加州大学伯克利分校的[詹妮弗·杜德纳](https://zh.wikipedia.org/wiki/珍妮弗·道德纳)和瑞典于默奥大学的[艾曼纽·卡彭蒂耶](https://zh.wikipedia.org/wiki/埃马纽埃尔·卡彭蒂耶)在《科学》杂志上发表了一篇划时代的论文，首次证明CRISPR-Cas9系统可以被重新编程为一种通用的基因编辑工具。这一发现源于对细菌免疫系统的基础研究——她们发现细菌用CRISPR序列来"记住"入侵的病毒DNA，并利用Cas9蛋白精确切割匹配的DNA序列。

杜德纳回忆说，当她们第一次在试管中看到Cas9能够精确切割DNA时，"那一刻，我们都知道世界将从此改变"。她们很快意识到这项技术不仅可以用于基础研究，更有可能治愈遗传病。

2020年，杜德纳和卡彭蒂耶因CRISPR基因编辑技术荣获诺贝尔化学奖，这是科学史上首次由两位女性科学家单独共享一项诺贝尔科学奖。从基础发现到临床应用（Casgevy于2023年获批）仅用了11年，这在医学史上是前所未有的速度。

### 詹姆斯·威尔逊：AAV载体的先驱

[詹姆斯·威尔逊](https://en.wikipedia.org/wiki/James_M._Wilson_(geneticist))是宾夕法尼亚大学的遗传学家，是AAV载体技术的奠基人之一。在1999年[杰西·格尔辛格](https://en.wikipedia.org/wiki/Jesse_Gelsinger)悲剧发生后，作为该临床试验的负责人，威尔逊承受了巨大的压力和指责。他一度被禁止领导临床试验长达五年。

然而，威尔逊没有被击倒。他深刻反思了腺病毒载体的安全问题，转而投入AAV载体的研究。他的团队系统性地发现了数十种新型AAV血清型，并开发了组织特异性定向载体，极大地拓展了AAV在基因治疗中的应用范围。今天，绝大多数获批的in vivo基因治疗药物都使用AAV载体，威尔逊的贡献功不可没。他的故事是科学史上"从失败中重生"的经典案例。

---

## 五、重要文献

1. **Friedmann, T. & Roblin, R. (1972)**. "Gene Therapy for Human Genetic Disease?" *Science*, 175(4025), 949-955.  
   → 首次正式提出基因治疗概念框架的开创性论文，奠定了整个领域的理论基础。

2. **Blaese, R.M. et al. (1995)**. "T Lymphocyte-Directed Gene Therapy for [ADA-SCID](https://en.wikipedia.org/wiki/Adenosine_deaminase_deficiency): Initial Trial Results After 4 Years." *Science*, 270(5235), 475-480.  
   → 人类第一例基因治疗临床试验的正式报告，证明[ex vivo](https://en.wikipedia.org/wiki/Gene_therapy#Ex_vivo)基因治疗在人体中的可行性。

3. **Jinek, M. et al. (2012)**. "A Programmable Dual-RNA-Guided DNA Endonuclease in Adaptive Bacterial Immunity." *Science*, 337(6096), 816-821.  
   → 杜德纳和卡彭蒂耶证明CRISPR-Cas9可编程基因编辑的里程碑论文。

4. **Frangoul, H. et al. (2021)**. "CRISPR-Cas9 Gene Editing for Sickle Cell Disease and β-Thalassemia." *New England Journal of Medicine*, 384(3), 252-260.  
   → Casgevy的关键临床试验结果，证明CRISPR基因编辑在人类遗传病治疗中的有效性。

5. **Mendell, J.R. et al. (2020)**. "Current Clinical Applications of In Vivo Gene Therapy with AAVs." *Molecular Therapy*, 28(4), 1041-1054.  
   → 系统综述AAV载体基因治疗的临床应用现状。

6. **NCBI PMC文献**："Viral vector-based gene therapies in the clinic: An update" (2025)  
   → 全面更新了截至2025年全球获批基因治疗药物的载体类型、适应症和给药途径。详见 [NCBI PMC](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12821227/)。

7. **NCBI PMC文献**："Gene Therapy Techniques and Delivery Methods (Review)" (2025)  
   → 综述了基因编辑技术的最新进展，包括2iHDR技术和紧凑型基因组编辑器。详见 [NCBI PMC](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12892848/)。

---

## 六、经典实验

### 实验一：人类第一例基因治疗（1990年）

**研究者**：[威廉·弗伦奇·安德森](https://en.wikipedia.org/wiki/W._French_Anderson)、迈克尔·布莱斯、肯尼斯·卡尔弗  
**对象**：4岁ADA-SCID患儿阿珊蒂·德席尔瓦  

**实验设计**：
1. 从患者外周血中提取T淋巴细胞
2. 使用逆转录病毒载体将正常ADA基因导入T细胞
3. 将基因修饰后的T细胞扩增培养
4. 通过静脉输注将修饰细胞回输到患者体内

**结果**：治疗后患者的ADA酶活性显著升高，T细胞数量和功能明显改善。虽然患者仍需配合PEG-ADA酶替代治疗，但其免疫功能得到了实质性的提升。这一实验证明了基因治疗在人体中的安全性和可行性，开辟了一个全新的医学领域。

**意义**：这是人类医学史上的里程碑事件，首次证明了通过基因操作可以治疗遗传性疾病。

### 实验二：Casgevy的CTX001临床试验（2019-2023）

**研究者**：Vertex Pharmaceuticals与CRISPR Therapeutics联合团队  
**对象**：[镰状细胞病](https://zh.wikipedia.org/wiki/镰状细胞病)和β-[地中海贫血](https://zh.wikipedia.org/wiki/地中海贫血)患者  

**实验设计**：
1. 从患者体内采集[造血干细胞](https://zh.wikipedia.org/wiki/造血幹細胞)（[HSC](https://en.wikipedia.org/wiki/Hematopoietic_stem_cell_transplantation)）
2. 使用CRISPR-Cas9编辑BCL11A基因的增强子区域，解除对胎儿血红蛋白（HbF）的抑制
3. 患者接受清淋预处理（白消安）
4. 将编辑后的造血[干细胞](https://zh.wikipedia.org/wiki/幹細胞)回输到患者体内
5. 编辑后的细胞重新激活胎儿血红蛋白的产生，替代缺陷的成人血红蛋白

**结果**：在[镰状细胞病](https://zh.wikipedia.org/wiki/镰状细胞病)患者中，94.1%的患者在治疗后至少12个月内无血管闭塞危象（VOC）发作。在β-[地中海贫血](https://zh.wikipedia.org/wiki/地中海贫血)患者中，91.4%的患者实现了摆脱输血依赖。这些结果发表在《新英格兰医学杂志》上，引起了全球轰动。

**意义**：这是全球首个基于CRISPR基因编辑的获批疗法，标志着基因编辑技术从实验室走向临床的里程碑。2023年12月，FDA正式批准Casgevy用于治疗镰状细胞病和输血依赖型β-地中海贫血。2026年7月，FDA进一步扩展适应症至2岁以上儿童，使约5500名患者首次有机会接受治疗。

### 实验三：Luxturna的III期临床试验

**研究者**：Spark Therapeutics团队  
**对象**：RPE65基因突变导致的Leber先天性黑矇（LCA）患者  

**实验设计**：通过视网膜下注射将携带正常RPE65基因的AAV2载体直接递送到视网膜色素上皮细胞。这是一个in vivo基因治疗的经典案例。

**结果**：接受治疗的患者在多亮度迷宫测试中的表现显著改善，视觉功能得到可测量的提升。截至2025年，Luxturna已在全球范围内帮助超过400名患者改善了视力。

**意义**：Luxturna是FDA批准的首个直接给药的遗传性失明基因治疗药物（2017年），也是首个in vivo基因治疗药物，证明了AAV载体在体内基因递送中的安全性和有效性。

---

## 七、小故事

### "一针210万美元"的Zolgensma

2019年，诺华公司的Zolgensma获批上市，用于治疗[脊髓性肌萎缩症](https://zh.wikipedia.org/wiki/脊髓性肌萎縮症)（SMA）——一种在婴儿中致死率极高的遗传性神经肌肉疾病。Zolgensma的定价为210万美元一剂，创下了当时全球最贵药物的纪录。

这个天价引发了广泛的社会讨论：基因治疗到底该值多少钱？支持者指出，Zolgensma是一次性治疗，而传统的SMA治疗药物Spinraza第一年费用高达75万美元，此后每年还需37.5万美元，终身治疗费用远超Zolgensma。反对者则质疑，即便是一次性治疗，如此高昂的价格也使得大多数患者家庭无法承受。

这场讨论揭示了基因治疗面临的一个核心困境：技术上的突破性进步如何转化为可及的医疗资源？如今，Zolgensma已在50多个国家获批，诺华也建立了抽奖赠药项目，每年为全球100名SMA患儿提供免费治疗。但"天价药"问题仍然是基因治疗产业发展中亟待解决的难题。

### 杰西·格尔辛格：以生命推动科学进步

1999年9月，18岁的杰西·格尔辛格患有一种温和的鸟氨酸氨甲酰转移酶（OTC）缺乏症，通过饮食和药物控制良好。他自愿参加了宾夕法尼亚大学的基因治疗临床试验，希望能帮助其他更严重的OTC缺乏症患者。

试验使用的是腺病毒载体，在动物实验中表现良好。然而，格尔辛格在接受注射后出现了剧烈的免疫反应——全身炎症反应综合征（SIRS），四天后因多器官衰竭去世。

事后调查发现，试验团队在知情同意过程中没有充分告知风险，且在格尔辛格肝功能异常时未能及时中止试验。FDA对该研究团队进行了严厉处罚，首席研究员[詹姆斯·威尔逊](https://en.wikipedia.org/wiki/James_M._Wilson_(geneticist))被禁止领导临床试验五年。

格尔辛格的父亲后来成为基因治疗安全监管的积极推动者。他说："我不希望杰西的死毫无意义。"正是这场悲剧推动了基因治疗临床试验监管的全面改革，加速了更安全的AAV载体取代腺病毒载体，最终为基因治疗的成功铺平了道路。

### Casgevy与"第一次"的意义

2023年12月8日，当FDA批准Casgevy的消息传出时，CRISPR Therapeutics的联合创始人[艾曼纽·卡彭蒂耶](https://zh.wikipedia.org/wiki/埃马纽埃尔·卡彭蒂耶)正在实验室里。她后来回忆说，那一刻她想起了2012年发表CRISPR论文时的情景："当时我们知道自己发现了一件重要的事，但从未想过仅仅11年后它就能成为获批准的药物，真正治愈患者。"

Casgevy的成功意味着，CRISPR基因编辑不再只是实验室中的工具，而是一种可以改变患者命运的治疗手段。对于镰状细胞病患者来说，这意味着终结终身的疼痛危机和输血依赖；对于科学家来说，这标志着[精准医学](https://zh.wikipedia.org/wiki/精准医学)新时代的开始。2026年7月，FDA进一步将Casgevy的适应症扩展至2岁以上儿童，使这项技术惠及更年轻的患者群体——从概念到惠及幼儿，基因治疗用了不到36年。

---

## 八、思考题

1. **ex vivo与in vivo的权衡**：为什么Casgevy选择ex vivo策略而Luxturna选择in vivo策略？如果你是一名基因治疗研发人员，面对一种肝脏遗传病和一种血液病，你会分别选择哪种策略？请从靶向效率、安全性、可操作性等角度分析。

2. **免疫原性挑战**：AAV载体虽然在多数患者中安全性良好，但部分患者体内存在预存的中和抗体，会阻止载体进入细胞。请思考：如何解决AAV载体的免疫原性问题？免疫抑制剂的使用有哪些利弊？

3. **[脱靶效应](https://en.wikipedia.org/wiki/Off-target_genome_editing)与安全性**：CRISPR-Cas9的[脱靶效应](https://en.wikipedia.org/wiki/Off-target_genome_editing)是基因编辑治疗中的核心安全顾虑。碱基编辑和先导编辑如何降低脱靶风险？你认为在临床应用中，可接受的脱靶率应该是多少？

4. **伦理边界**：体细胞基因治疗（如Casgevy）只影响患者本人，而生殖细胞基因编辑（如贺建奎事件中的胚胎编辑）会影响后代。请讨论：在什么条件下（如果有的话），生殖细胞基因编辑是可以接受的？国际社会应如何建立共识？

5. **可及性与公平**：Zolgensma定价210万美元，Casgevy定价220万美元。基因治疗的高昂成本使得许多患者无法负担。请思考：如何平衡创新激励与患者可及性？政府、保险公司和制药企业各自应承担什么责任？

6. **技术展望**：截至2025年12月，全球有136项CRISPR临床试验正在进行，其中36项基于体内递送，且非病毒载体比例上升。你认为未来10年基因治疗的最大突破将出现在哪个方向？是新的递送技术、新的编辑工具，还是新的疾病适应症？

---

## 九、术语表

| 术语 | 英文 | 释义 |
|------|------|------|
| 基因治疗 | Gene Therapy | 通过将遗传物质导入患者细胞来治疗或预防疾病的技术 |
| ex vivo | Ex vivo gene therapy | 将细胞从体内取出、在体外进行基因改造后回输的策略 |
| in vivo | In vivo gene therapy | 将基因治疗载体直接注射到患者体内的策略 |
| AAV | Adeno-Associated Virus | [腺相关病毒](https://zh.wikipedia.org/wiki/腺相关病毒)，一种免疫原性低、可长期表达的小型DNA病毒，是基因治疗最常用的载体 |
| [慢病毒载体](https://en.wikipedia.org/wiki/Lentivirus) | Lentiviral Vector | 源自HIV的改造载体，可感染分裂和非分裂细胞，常用于CAR-T细胞治疗 |
| 造血[干细胞](https://zh.wikipedia.org/wiki/幹細胞) | Hematopoietic Stem Cell (HSC) | 存在于骨髓中的干细胞，可分化为所有类型的血细胞 |
| CAR-T | Chimeric Antigen Receptor T-cell | 嵌合抗原受体T细胞，通过基因改造T细胞使其识别并杀伤癌细胞 |
| [基因增强](https://en.wikipedia.org/wiki/Gene_therapy#Gene_augmentation) | Gene Augmentation | 导入正常基因拷贝以补偿缺陷基因功能的策略 |
| 基因编辑 | Gene Editing | 使用CRISPR等工具在基因组层面进行精确修改的技术 |
| 碱基编辑 | Base Editing | 在不产生DNA双链断裂的情况下实现单碱基转换的基因编辑技术 |
| 先导编辑 | Prime Editing | 实现"搜索-替换"式基因编辑，可进行所有类型碱基替换和小片段插入缺失 |
| [脂质纳米颗粒](https://zh.wikipedia.org/wiki/脂质纳米颗粒) | Lipid Nanoparticle (LNP) | 用于递送核酸的非病毒载体，在mRNA疫苗中成功应用 |
| 脱靶效应 | Off-target Effect | 基因编辑工具在非目标位点产生意外编辑的现象 |
| 免疫原性 | Immunogenicity | 治疗载体或产物引发免疫反应的能力 |
| 清淋预处理 | Myeloablative Conditioning | 在造血干细胞移植前使用化疗药物清除患者原有骨髓细胞的过程 |
| ADA-SCID | ADA-SCID | 腺苷脱氨酶缺陷导致的重症联合免疫缺陷，又称"泡泡男孩病" |
| 镰状细胞病 | Sickle Cell Disease (SCD) | 由β-珠蛋白基因突变导致的遗传性血液病，红细胞呈镰刀状 |
| β-地中海贫血 | β-Thalassemia | β-珠蛋白基因突变导致血红蛋白合成不足的遗传性血液病 |
| 胎儿血红蛋白 | Fetal Hemoglobin (HbF) | 胎儿期表达的血红蛋白，出生后通常被成人血红蛋白取代 |
| RPE65 | RPE65 Gene | 视网膜色素上皮65基因，其突变导致Leber先天性黑矇 |

---

## 十、下节预告

### Day 91：转基因技术

明天我们将进入[转基因](https://zh.wikipedia.org/wiki/转基因)技术的世界。如果说基因治疗是将基因导入人体细胞来治疗疾病，那么[转基因](https://zh.wikipedia.org/wiki/转基因)技术则是将外源基因导入生物体来赋予其新的性状。从转基因作物（抗虫棉、黄金大米）到转基因动物（转基因鲑鱼、基因修饰猪），转基因技术正在深刻改变农业、医药和工业的面貌。

我们将探讨：
- 转基因技术的基本原理与常用方法（农杆菌介导法、基因枪法、CRISPR介导的精准转基因）
- 转基因作物的安全性争议与社会讨论
- 转基因动物在异种器官移植中的前景
- 转基因技术面临的伦理挑战与监管框架

从治病到改物，基因技术正在以前所未有的广度重塑生命世界。敬请期待！

---

> **📖 遗传学100天学习计划**  
> Day 90 / 100 · 基因治疗的进展  
> *坚持学习，每日精进。离完成100天还有10天。*

---

## 📚 综合学习资源链接

> 以下为本节核心知识点的精选学习资源，涵盖多语言和多平台。

### 🔬 核心概念资源

| 主题 | Wikipedia | YouTube | B站 | NCBI |
|------|-----------|---------|-----|------|
| [基因治疗](https://zh.wikipedia.org/wiki/基因治疗) | [中文](https://zh.wikipedia.org/wiki/基因治疗) / [English](https://en.wikipedia.org/wiki/Gene_therapy) | [搜索](https://www.youtube.com/results?search_query=gene+therapy+explained) | [搜索](https://search.bilibili.com/all?keyword=基因治疗) | [NCBI Bookshelf](https://www.ncbi.nlm.nih.gov/books/NBK115571/) |
| [CRISPR-Cas9](https://zh.wikipedia.org/wiki/CRISPR) | [中文](https://zh.wikipedia.org/wiki/CRISPR) / [English](https://en.wikipedia.org/wiki/CRISPR) | [视频讲解](https://www.youtube.com/watch?v=2pp7E5-qV1Q) | [搜索](https://search.bilibili.com/all?keyword=CRISPR+Cas9) | [NCBI](https://www.ncbi.nlm.nih.gov/books/NBK447249/) |
| [AAV载体](https://zh.wikipedia.org/wiki/腺相关病毒) | [中文](https://zh.wikipedia.org/wiki/腺相关病毒) | [搜索](https://www.youtube.com/results?search_query=AAV+vector) | [搜索](https://search.bilibili.com/all?keyword=AAV载体) | [PMC](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12341529/) |
| [CAR-T细胞治疗](https://zh.wikipedia.org/wiki/CAR-T细胞) | [中文](https://zh.wikipedia.org/wiki/CAR-T细胞) | [视频](https://www.youtube.com/watch?v=ErkQuZFU5E0) | [搜索](https://search.bilibili.com/all?keyword=CAR-T) | [NCBI](https://www.ncbi.nlm.nih.gov/books/NBK536951/) |

### 💊 已批准基因治疗药物

| 药物名称 | 适应症 | 批准年份 | FDA链接 | Wikipedia |
|----------|--------|----------|---------|-----------|
| Casgevy | 镰状细胞病/地中海贫血 | 2023 | [FDA](https://www.fda.gov/news-events/press-announcements/fda-approves-first-gene-therapy-young-children-sickle-cell-disease) | [Wiki](https://en.wikipedia.org/wiki/Exagamglogene_autotemcel) |
| Luxturna | Leber先天性黑矇 | 2017 | [FDA](https://www.fda.gov/vaccines-blood-biologics/cellular-gene-therapy-products/luxturna) | [Wiki](https://en.wikipedia.org/wiki/Voretigene_neparvovec) |
| Zolgensma | 脊髓性肌萎缩症 | 2019 | [FDA](https://www.fda.gov/news-events/press-announcements/fda-approves-novel-gene-therapy-treat-pediatric-patients-spinal-muscular-atrophy) | [Wiki](https://en.wikipedia.org/wiki/Onasemnogene_abeparvovec) |
| Elevidys | 杜氏肌营养不良 | 2023 | [FDA](https://www.fda.gov/news-events/press-announcements/fda-grants-accelerated-approval-first-gene-therapy-treat-duchenne-muscular) | [Wiki](https://en.wikipedia.org/wiki/Delandistrogene_moxeparvovec) |
| Hemgenix | 血友病B | 2022 | [FDA](https://www.fda.gov/news-events/press-announcements/fda-approves-first-gene-therapy-treat-adults-hemophilia-b) | [Wiki](https://en.wikipedia.org/wiki/Etranacogene_dezaparvovec) |
| Roctavian | 血友病A | 2023 | [FDA](https://www.fda.gov/news-events/press-announcements/fda-approves-first-gene-therapy-hemophilia) | [Wiki](https://en.wikipedia.org/wiki/Valoctocogene_roxaparvovec) |

### 📖 推荐阅读文献

1. **Viral vector-based gene therapies in the clinic: An update** - [NCBI PMC](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12821227/)
2. **Gene Therapy Techniques and Delivery Methods (Review)** - [NCBI PMC](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12892848/)
3. **Non-Viral CRISPR carriers: transient delivery with lasting effects** - [NCBI PMC](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12818331/)
4. **Base and Prime Editing for Inherited Retinal Diseases** - [NCBI PMC](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12655462/)
5. **AAV-delivered gene editing therapeutics for CNS disorders** - [NCBI PMC](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12341529/)

### 🎬 推荐视频资源

| 平台 | 资源名称 | 链接 |
|------|----------|------|
| YouTube | Gene Therapy Explained | [观看](https://www.youtube.com/results?search_query=gene+therapy+explained) |
| YouTube | CRISPR-Cas9 Mechanism | [观看](https://www.youtube.com/watch?v=2pp7E5-qV1Q) |
| YouTube | CAR-T Cell Therapy | [观看](https://www.youtube.com/watch?v=ErkQuZFU5E0) |
| B站 | 基因治疗科普 | [观看](https://search.bilibili.com/all?keyword=基因治疗) |
| B站 | CRISPR基因编辑 | [观看](https://search.bilibili.com/all?keyword=CRISPR基因编辑) |

---

*📅 本资源列表由 workflow.py 自动生成于 Day 90 - 基因治疗的进展*
