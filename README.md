### neo4j图谱
- 实体数量：206466
- 实体种类：22类
- 关系数量：71418
- 关系种类：16类
##Taxonomy
如果没有概念的分类系统，概念则是一堆散沙，无法通过结构来形成系统的能力。
Taxonomy源自希腊文，Taxis表示整理或安排，而Nomos意味法则或规则。在《大美百科全书》中taxonomy是“生物分类学”的意思，其是生物分门别类的工作及理论。在《简明大英百科全书》中则译为“分类学”，指的也是生物学上将有机体从一般到特殊分成不同的层次组别，以反映演化和形态关联。
早先在图书资讯学领域taxonomy通常被理解为分类（classification），且主要是用在生命科学上。但逐渐taxonomy在资讯检索的领域中也常被使用，因为各家用法不同，导致taxonomy究竟是一种分类表或是一种索引典而引起困惑。Taxonomy有多种中文译法，除“学科分类学”外，近来有学者将taxonomy译成“知识分类学”或“知识分类表”。回溯知识分类学用法，最早是由“逻辑之父”亚里斯多德，用来组织并深化其周遭世界的知识。亚里斯多德的方法被文艺复兴时代和启蒙时代的科学家所沿用，如瑞典的博物学家林奈（Linnaeus），他使用相同的技巧进行生物分类，经过修改，广泛地沿用至今。林奈的分类是典型的知识分类学，生物间的关係是以阶层式（hierarchical）的结构描述。这个连续的阶层结构在阶层划分中产生出更小或更专指的类。它通常视觉化地呈现为树状结构，在每一个新的阶层中有树的分支，这种结构通常被认为是分类的系统。taxonomy不只专门应用在自然科学领域，现今被广泛的应用在其他数个学科，包括：社会科学、计算机和信息科学、语言学、认知科学、网站设计与建构（例如：Yahoo!入口网站，其分类表是taxonomy原型例子之一）。在这些领域中，taxonomy具有多元的意义，不再被限制于传统生物学的意义。1990年代，taxonomy被重新定义为“任何语义上的特殊意义”，如内容的系统化组织，或发展此种系统化组织的过程。
Taxonomy知识分类的科学或技巧，是由范畴（category）和连结范畴的关係所组成的一种架构；是将业务对象与事先定义好的标签配对（matching）的过程；是一个树型得分类表／分类系统／标签系统；是知识地图。Classification scheme ／system和taxonomy经常被交替使用，但通常来说classification scheme／system的产生是从上到下（top-down），根据主题，向下复分，所以是“主动的”（分类的主要目的是指引使用者找到资讯的主体）；taxonomy是从下到上（bottom-up）、从各种学问的实际内容产生，比起classification scheme／system，它是更实用。
4.2.3 分类设计原则2
我们将搜集和总结得企业概念（Concepts）形成分类体系（Taxonomies），形成一个初步的知识地图。
分类设计参考以下一些原则。
•	确定分类的目的。
•	确定分类法的候选者。
•	遵循MECE 原则（相互排斥，完全穷尽）。
•	考虑层级或级别的同质性。
•	决定是否在所有情况下都需要叶类别。
•	识别不需要分类法的属性和属性。
- 确定分类目的
分类法设计的一个关键方面是分类法的目的。分类法的目的特定于其消费者受众。
例如，您可以使用分类法来帮助采购负责人了解年度支出。这种分类法需要将交易分类为反映供应市场高层次细分的广泛类别。
在我们的业务场景下，分类是帮助营销人员来了解“顾客要什么”，“我们有什么”的问题。需要将我们场景里的数字资产从产品，市场，地域等方面分类细分。
- 确定分类的候选对象
围绕实现分类目的，确定要分类对象：尽早澄清任何歧义可以实现一致的分类。

- MECE 原则
每个分类体系中所列举的概念，根据个体互斥、集体穷举的MECE(Mutually Exclusive, Collectively Exhaustive) 原则安排。即每一个并列的概念互相之间没有重合，而所有并列的概念在一起覆盖了整个分类对象。不重不漏。分类法越遵循此原则，就越容易用于对记录进行分类。虽然 MECE 在实践中很难实现，但在设计分类时记住这一原则有助于确保每个业务对象都只归属一个也必归属于某一分类概念。
在我们的分类体系中，在地域等分类，能够较好地做到MECE。而在产品方案亮点特性和价值，在某些分类对象上，由于业务错综复杂，快速消长，不具备业务概念定义权，业务语言缺乏标准等实际原因，无法彻底实现MECE。这对后续的数据处理，搜索推荐等算法提出了更高的要求。
- 考虑层级或级别同质性
分类系统同层内的概念应该是统一种类。
以例如生物分类法，其中所有同层类别都分别属于同门、同纲、同目、同科、同属或同种。对于绝大多数分类法，不可能实现完美的层同质性。MECE 原则适用于层内的组，就像适用于跨层的类别一样。取而代之的是，分类法的目标应该是拥有尽可能少的层级非同质组。

```mermaid
flowchart TD;
     A-->B;
     A-->C;
     B-->D;
     C-->D;
