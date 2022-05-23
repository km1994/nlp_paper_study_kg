# 【关于 NLP】 那些你不知道的事 ———— 知识图谱篇

> 作者：杨夕
> 
> 介绍：研读顶会论文，复现论文相关代码
> 
> NLP 百面百搭 地址：https://github.com/km1994/NLP-Interview-Notes
> 
> **[手机版NLP百面百搭](https://mp.weixin.qq.com/s?__biz=MzAxMTU5Njg4NQ==&mid=100005719&idx=3&sn=5d8e62993e5ecd4582703684c0d12e44&chksm=1bbff26d2cc87b7bf2504a8a4cafc60919d722b6e9acbcee81a626924d80f53a49301df9bd97&scene=18#wechat_redirect)**
> 
> 推荐系统 百面百搭 地址：https://github.com/km1994/RES-Interview-Notes
> 
> **[手机版推荐系统百面百搭](https://mp.weixin.qq.com/s/b_KBT6rUw09cLGRHV_EUtw)**
> 
> 搜索引擎 百面百搭 地址：https://github.com/km1994/search-engine-Interview-Notes 【编写ing】
> 
> NLP论文学习笔记：https://github.com/km1994/nlp_paper_study
> 
> 推荐系统论文学习笔记：https://github.com/km1994/RS_paper_study
> 
> GCN 论文学习笔记：https://github.com/km1994/GCN_study
> 
> **推广搜 军火库**：https://github.com/km1994/recommendation_advertisement_search
![](other_study/resource/pic/微信截图_20210301212242.png)

> 手机版笔记，可以关注公众号 **【关于NLP那些你不知道的事】** 获取，并加入 【NLP && 推荐学习群】一起学习！！！

> 注：github 网页版 看起来不舒服，可以看 **[手机版NLP论文学习笔记](https://mp.weixin.qq.com/s?__biz=MzAxMTU5Njg4NQ==&mid=100005719&idx=1&sn=14d34d70a7e7cbf9700f804cca5be2d0&chksm=1bbff26d2cc87b7b9d2ed12c8d280cd737e270cd82c8850f7ca2ee44ec8883873ff5e9904e7e&scene=18#wechat_redirect)**

- [【关于 NLP】 那些你不知道的事 ———— 知识图谱篇](#关于-nlp-那些你不知道的事--知识图谱篇)
  - [介绍](#介绍)
    - [NLP 学习篇](#nlp-学习篇)
      - [理论学习篇](#理论学习篇)
        - [【关于 知识图谱 】 那些的你不知道的事](#关于-知识图谱--那些的你不知道的事)
          - [【关于 实体链指篇】 那些的你不知道的事](#关于-实体链指篇-那些的你不知道的事)
          - [【关于 实体消歧】 那些的你不知道的事](#关于-实体消歧-那些的你不知道的事)
          - [【关于KGQA】 那些的你不知道的事](#关于kgqa-那些的你不知道的事)
          - [【关于Neo4j】 那些的你不知道的事](#关于neo4j-那些的你不知道的事)
          - [【关于 知识图谱补全(图谱推理) 】 那些的你不知道的事](#关于-知识图谱补全图谱推理--那些的你不知道的事)
  - [参考资料](#参考资料)

## 介绍

### NLP 学习篇

#### 理论学习篇

##### [【关于 知识图谱 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/)

- [【关于 知识图谱 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/)
  - 一、知识图谱简介
    - 1.1 引言
    - 1.2 什么是知识图谱呢？
      - 1.2.1 什么是图（Graph）呢？
      - 1.2.2 什么是 Schema 呢？
    - 1.3 知识图谱的类别有哪些？
    - 1.4 知识图谱的价值在哪呢？
  - 二、怎么构建知识图谱呢？
    - 2.1 知识图谱的数据来源于哪里？
    - 2.2 信息抽取的难点在哪里？
    - 2.3 构建知识图谱所涉及的技术？
    - 2.4、知识图谱的具体构建技术是什么？
      - 2.4.1 实体命名识别（Named Entity Recognition）
      - 2.4.2 关系抽取（Relation Extraction）
      - 2.4.3 实体统一（Entity Resolution）
      - 2.4.4 指代消解（Disambiguation）
  - 三、知识图谱怎么存储？
  - 四、知识图谱可以做什么？
- [爱奇艺知识图谱落地实践](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/爱奇艺知识图谱落地实践/)
  - 原文地址：[领域应用 | 完备的娱乐行业知识图谱库如何建成？爱奇艺知识图谱落地实践](https://mp.weixin.qq.com/s?__biz=MzU2NjAxNDYwMg==&mid=2247493658&idx=1&sn=cc2d7f82aa5c5a138dc7f267aaa26c16&chksm=fcb04fffcbc7c6e9575f5dcc3d1619425e4dd7fc0737976991bff687af6b1dadcdd20f906d04&mpshare=1&scene=22&srcid=0809aEdiDZ0DSoxjfzSF8Kcf&sharer_sharetime=1628471753625&sharer_shareid=da84f0d2d31380d783922b9e26cacfe2#rd)
  - 构建流程
    - 知识表示和建模：自顶向下的建模方式
    - 数据模式（schema）定义方式：
      - 基于 RDF(Resource Description Framework) 三元组
      - RDFS（RDF Schema） 的规则
    - 知识获取
      - 实体分类
        - 动机：主要**针对百度百科的数据**，因为**百度百科的数据没有类别信息**
        - 思路：
          - 构建基于规则池的分类器，生成训练数据，训练DNN模型（self-attention）文本分类模型；
          - DNN分类器与规则分类器互相扩充迭代（一到两轮），最终线上使用规则分类器。
      - 实体抽取
        - 目标：从数据中的识别和抽取实体的属性与关系信息
      - 知识融合
        - 流程：
          - 首先我们所有来源的实体数据都会进入原始实体库（RawEntity库），并且对原始表中的数据建立索引。
          - 当一个原始实体rawEntity入最终实体库之前，要在原始实体库中找是否有其它原始实体和rawEntity实际上是同一个实体。步骤：
            - 首先在索引中根据名字、别名等字段查询出若干个可能是相同实体的候选列表，这个步骤的目的是减少接下来流程的计算量。
            - 然后经过实体判别模型，根据模型得分识别出待合并对齐的原始实体；
            - 最后经过属性融合模型，将各原始实体的属性字段进行融合，生成最终的实体。
          - 这个流程中的合并判断模型实际上是通过机器学习训练生成的二分类器。
      - 知识存储

###### [【关于 实体链指篇】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/entity_linking/)
- [【关于  Low-resource Cross-lingual Entity Linking】 那些你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/entity_linking/LowResourceCrossLingualEntityLinking/)
  - 论文名称：Design Challenges in Low-resource Cross-lingual Entity Linking
  - 论文地址：https://arxiv.org/pdf/2005.00692.pdf
  - 来源：EMNLP 2020
- [【关于  GENRE】 那些你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/entity_linking/GENRE_ICLR21/)
  - 论文名称：AUTOREGRESSIVE ENTITY RETRIEVAL
  - 论文地址：https://openreview.net/pdf?id=5k8F6UU39V
  - 来源：ICLR 2021
  - 论文代码：https://github.com/facebookresearch/GENRE
  - 介绍：实体是我们表示和聚合知识的中心。例如，维基百科等百科全书是由实体构成的（例如，一篇维基百科文章）。检索给定查询的实体的能力是知识密集型任务（如实体链接和开放域问答）的基础。理解当前方法的一种方法是将分类器作为一个原子标签，每个实体一个。它们的权重向量是通过编码实体元信息（如它们的描述）产生的密集实体表示。
  - 缺点：
    - （i）上下文和实体的亲和力主要是通过向量点积来获取的，可能会丢失两者之间的细粒度交互；
    - （ii）在考虑大型实体集时，需要大量内存来存储密集表示；
    - （iii）必须在训练时对一组适当硬的负面数据进行二次抽样[。
  - 工作内容介绍：在这项工作中，我们提出了第一个 GENRE，通过生成其唯一的名称，从左到右，token-by-token 的自回归方式和条件的上下文。
  - 这使得我们能够缓解上述技术问题，
    - （i）自回归公式允许我们直接捕获文本和实体名称之间的关系，有效地交叉编码两者 ；
    - （ii）由于我们的编码器-解码器结构的参数随词汇表大小而不是词汇量大小而缩放，因此内存足迹大大减少实体计数；
    - （iii）准确的softmax损失可以有效地计算，而无需对负数据进行子采样。
  - 实验结果：我们展示了该方法的有效性，在实体消歧、端到端实体链接和文档检索任务上对20多个数据集进行了实验，在使用竞争系统内存占用的一小部分的情况下，获得了最新的或非常有竞争力的结果。他们的实体，我们只需简单地指定新的名称，就可以添加

###### [【关于 实体消歧】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/EntityDisambiguation/)

- [【关于 DeepType 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/EntityDisambiguation/DeepType/)
  - 论文：DeepType: Multilingual Entity Linking by Neural Type System Evolution
  - 论文地址：https://arxiv.org/abs/1802.01021
  - github：https://github.com/openai/deeptype

###### [【关于KGQA】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/KGQA/)

- [【关于KGQA】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/KGQA/)
  - 一、基于词典和规则的方法
  - 二、基于信息抽取的方法
- [【关于 Multi-hopComplexKBQA 】 那些你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/KGQA/ACL20_Multi-hopComplexKBQA/)
  - 论文：Lan Y, Jiang J. Query Graph Generation for Answering Multi-hop Complex Questions from Knowledge Bases[C]//Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics. 2020: 969-974.
  - 会议：ACL2020
  - 链接：https://www.aclweb.org/anthology/2020.acl-main.91/
  - 代码：https://github.com/lanyunshi/Multi-hopComplexKBQA
- [【关于 Complex KBQA】 那些你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/ComplexKBQA/)
  - 论文：A Survey on Complex Knowledge Base Question Answering:Methods, Challenges and Solutions
  - 会议：IJCAI'2021
  - 论文地址：https://www.ijcai.org/proceedings/2021/0611.pdf
  - 动机：
    - 相比仅包含单个关系事实的简单问题，复杂问题通常有以下几个特征
      - **需要在知识图谱中做多跳推理 (multi-hop reasoning)**
      - **需要考虑题目中给的限制词 (constrained relations)**
      - **需要考虑数字运算的情况 (numerical operations)**
    - **基于语义解析的方法还是信息检索的方法都将遇到新的挑战**：
      - **传统方法无法支撑问题的复杂逻辑**
      - **复杂问题包含了更多的实体，导致在知识图谱中搜索空间变大**
      - **两种方法都将问题理解作为首要步骤**
      - **通常 Complex KBQA 数据集缺少对正确路径的标注**
  - 预测答案两类主流的方法
    - 基于语义解析（SP-based）的方法
      - 问题理解 (question understanding) 模块
      - 逻辑解析 (logical parsing) 模块
      - 知识图谱实例化 (KB grounding) 模块
      - 知识执行 (KB execution) 模块
    - 基于信息检索（IR-based）的方法
      - 子图构建 (retrieval source construction) 模块
      - 问题表达 (question representation) 模块
      - 基于图结构的推理 (graph based reasoning) 模块
      - 答案排序 (answer ranking) 模块
- [【关于 子图检索增强的知识图谱问答方法】 那些你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/SubgraphRetrievalKBQA/)
  - 论文：Subgraph Retrieval Enhanced Model for Multi-hop Knowledge Base Question Answering
  - 会议：ACL2022
  - 链接：https://github.com/RUCKBReasoning/SubgraphRetrievalKBQA/tree/main/paper
  - 代码：https://github.com/RUCKBReasoning/SubgraphRetrievalKBQA
  - 背景：最近关于知识库问答 (KBQA) 的工作检索子图以便于推理。 
  - 动机：
    - 所需的子图至关重要，因为小的子图可能会排除答案，但大的子图可能会引入更多噪声。
    - 然而，现有的检索要么是启发式的，要么与推理交织在一起，导致对部分子图的推理，在缺少中间监督时增加了推理偏差。
  - 论文方法：本文提出了一种与后续推理过程分离的可训练子图检索器（SR），它使即插即用框架能够增强任何面向子图的 KBQA 模型。 
  - 实验结果：与现有检索方法相比，SR 取得了显着更好的检索和 QA 性能。 通过弱监督的预训练以及端到端的微调，SRl 与 NSM（一种面向子图的推理器）相结合，用于基于嵌入的 KBQA 方法，实现了新的最先进的性能。


###### [【关于Neo4j】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/neo4j/)

- [【关于Neo4j】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/neo4j/)
  - 一、Neo4J 介绍与安装
    - 1.1 引言
    - 1.2 Neo4J 怎么下载？
    - 1.3 Neo4J 怎么安装？
    - 1.4 Neo4J Web 界面 介绍
    - 1.5 Cypher查询语言是什么？
  - 二、Neo4J 增删查改篇
    - 2.1 引言
    - 2.2 Neo4j 怎么创建节点？
    - 2.3 Neo4j 怎么创建关系？
    - 2.4 Neo4j 怎么创建 出生地关系？
    - 2.5 Neo4j 怎么查询？
    - 2.6 Neo4j 怎么删除和修改？
  - 三、如何利用 Python 操作 Neo4j 图数据库？
    - 3.1 neo4j模块：执行CQL ( cypher ) 语句是什么？
    - 3.2 py2neo模块是什么？
  - 四、数据导入 Neo4j 图数据库篇

- [【关于 Neo4j 索引】那些你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/neo4j/index.md)

###### [【关于 知识图谱补全(图谱推理) 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/KG_reasoning/)

- [【关于 知识图谱补全】那些你不知道的事](https://github.com/km1994/nlp_paper_study_kg/tree/master/KG_study/KG_reasoning/)

- [【关于 基于逻辑规则的图谱推理 RNNLogic 】 那些你不知道的事]()
  - 论文：RNNLogic: Learning Logic Rules for Reasoning on Knowledge Graphs
  - 动机：
    - **图谱信息是不完全的**，而补全图谱的人工成本又是非常巨大的，尤其是像是一些医药、金融等一些特定的领域。如果还要考虑知识的动态更新的话，就更加大了图谱补全的难度。
    - 图谱表示法：模型缺乏可解释性
    - 归纳逻辑编程法：对规则的搜索空间大，因为固定的生成器。如果想要得到比较好的结果就要尝试大量的逻辑规则，导致效率较低。
    - 基于强化学习的方法：整个框架的优化很难；依赖KGE（图谱嵌入）的方法来做激励调整。
  - 论文思路：
    - 研究点 1：链式的逻辑规则：可以将链式的逻辑规则变成一个关系序列，其中用END来表示结尾。那很自然的，可以通过LSTM来生成这些不同的链式逻辑规则，并输出每一条逻辑规则的概率，进而得到一个弱逻辑规则的集合；
    - 研究点 2：随机逻辑编程（stochastic logic programming）：
      - 会通过生成器的弱关系集合进行游走，如图中所示的两种关系链：
        - 第一种可以得到France这个答案；
        - 第二个逻辑规则可以得到France，Canada和US三个答案。
      - 对于每个潜在答案，我们可以给它定义一个分数，也就是到达这个实体的逻辑规则的weight的和。
      - 最后就可以根据分数得到每种答案的概率，挑选出那些概率最大的来当成我们最终的答案。
    - 研究点 3：优化方法
      - 1. 给定一个查询（Query），让生成器生成很多逻辑规则，再把逻辑规则和知识图谱同时送到预测器里面，去更新预测器，最大化生成正确答案的概率；
      - 2. 从所有生成的这些逻辑规则里面去挑选出那些最重要的逻辑规则。这里我们通过使用后验推断的方法来计算每一条弱的逻辑规则的后验概率进行挑选。因此，在整个过程中，每一条弱的规则概率是由生成器来提供的，似然函数由预测器来提供。这样结合两者共同的信息来得到一个比较重要的逻辑规则；
      - 3. 把找到的高质量的逻辑规则当成训练数据，送回生成器去学习；

## 参考资料

1. [【ACL2020放榜!】事件抽取、关系抽取、NER、Few-Shot 相关论文整理](https://www.pianshen.com/article/14251297031/)
2. [第58届国际计算语言学协会会议（ACL 2020）有哪些值得关注的论文？](https://www.zhihu.com/question/385259014)
