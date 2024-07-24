# fundamentals-of-software-architecture 学习笔记

### 第一章
<img width="653" alt="image" src="https://github.com/user-attachments/assets/0f8fb6e9-c7a5-4ce3-91cf-01ccf2f8741f">
架构由结构、架构特征、设计原则组成

###### 1. 软件架构定义

结构：系统的结构包括架构风格（如微服务、分层架构等）​​。

架构特性：架构特性是系统必须支持的成功标准，通常与系统功能无关，但对系统正常运行至关重要​​。

架构决策：这些是系统应如何构建的规则。例如，架构师可能会决定在分层架构中，只有业务层和服务层可以访问数据库​​。

设计原则：设计原则是构建系统的指南，而不是硬性规定。例如，在微服务架构中使用异步消息传递以提高性能​​。

###### 2. 架构师的期望
架构师需要具备以下核心能力：

做出架构决策：引导而不是指定技术选择​​。

持续分析架构：确保架构在业务和技术变化中保持活力​​。

紧跟最新趋势：保持对最新技术和行业趋势的了解​​。

确保决策的合规性：确保开发团队遵循架构决策和设计原则​​。

广泛的技术和经验：至少熟悉多种技术​​。

商业领域知识：了解业务领域，以便更有效地设计架构​​。

人际交往能力：具备团队合作、协调和领导能力​​。

理解并驾驭公司政治：能够在企业的政治环境中有效地工作​​。

###### 3. 架构与其他领域的交集

工程实践：包括持续集成、自动化机器配置等​​。

运维/DevOps：架构与运维的紧密结合使得设计更加简化​​。

开发过程：软件开发过程（如敏捷开发）对架构有重要影响​​。

数据：数据架构是软件架构的重要组成部分，涉及如何存储和管理数据​​。

###### 4. 软件架构法则

第一法则：软件架构中的一切都是权衡取舍​​。

第二法则：理解为什么比理解如何更重要​​。


### 第二章 架构思维

##### 1. 架构与设计的区别


<img width="637" alt="image" src="https://github.com/user-attachments/assets/0db69e27-30ee-4a8f-aee1-4539080c12b5">


定义差异：架构和设计的区别常常引起混淆。架构涉及高层次的系统结构和全局决策，而设计关注实现这些结构的细节 。

传统职责分工：架构师负责分析业务需求、选择架构模式和创建系统组件，开发团队则负责具体的类图、用户界面和代码开发 。

协作需求：为了成功，架构师和开发团队必须紧密合作，确保架构设计和实现保持同步 。

#####  2. 技术广度

<img width="641" alt="image" src="https://github.com/user-attachments/assets/13ba8331-6d3b-4cde-bd9c-35da98b20bfe">

- 知识金字塔

技术知识的层次：技术知识可以分为三个层次：已知的知识（即技术深度）、已知的未知（知道自己不知道的知识）和未知的未知（不知道自己不知道的知识）。这三个层次共同构成了知识金字塔 。

已知的知识：指的是一个技术人员在日常工作中使用的技术、框架、语言和工具。例如，一个Java程序员对Java语言的掌握。

已知的未知：指的是技术人员听说过但不熟悉的技术。例如，许多技术人员知道Clojure是一种基于Lisp的编程语言，但可能并不精通。

未知的未知：指的是那些技术人员不知道它们存在，但实际上可能是解决当前问题的最佳方案的技术和工具。

- 技术人员的知识发展

开发人员的早期职业：开发人员在职业生涯的早期通常专注于扩展知识金字塔的顶端，即增加技术深度。这是因为开发人员需要更多的实践经验和操作知识来完成他们的工作 。
技术深度的维护：随着开发人员获得更多的经验，他们需要不断维护和更新他们的技术知识，因为技术在不断发展。例如，一个开发人员如果多年不使用某种技术，那么他们对该技术的掌握程度会逐渐减弱 。

- 架构师的技术广度

技术广度的重要性：架构师需要比开发人员拥有更广泛的技术知识，以便在不同的技术约束和业务需求下做出最佳决策。相比于单一的技术专长，广泛的技术知识更有助于架构师识别和应用最适合的技术解决方案 。

广度优先于深度：架构师应更加注重技术广度而不是深度。这意味着他们需要对多种技术、框架和工具有所了解，而不必精通每一种技术 。

技术广度的培养：架构师可以通过参与不同类型的项目、持续学习新技术和与其他技术专家交流来扩展他们的技术广度 。

- 角色转换中的挑战

从开发人员到架构师的过渡：开发人员在转变为架构师时，通常会面临一个从深度到广度的知识转换过程。这可能是一个具有挑战性的过程，因为这需要他们改变长期以来形成的专注于技术深度的思维模式 。
避免技术过时：架构师需要警惕其技术知识的过时性，即避免陷入“冰冻穴居人反模式”，即架构师依赖于过去的技术知识而忽略了新的技术发展 。

- 实践中的技术广度

技术广度的实际应用：在实际工作中，架构师需要广泛的技术知识来解决复杂的技术问题。例如，在选择缓存解决方案时，了解多种缓存产品及其优缺点会比只精通一种产品更有价值 。

##### 3. 权衡分析

不可避免的权衡：架构决策总是伴随着权衡，无法通过简单的搜索得到答案。每个架构问题的答案都依赖于具体的环境和需求 。
实例分析：例如，在竞拍系统中，选择使用队列还是主题进行消息传递，架构师需要根据具体情况分析两者的优缺点 。

##### 4. 理解业务驱动因素

业务需求转换：架构师需要将业务需求转化为架构特性（如可扩展性、性能和可用性），这需要对业务领域的深入理解和与业务利益相关者的紧密合作 。

##### 5. 平衡架构与实践编码

保持技术深度：架构师应保持一定的编码实践，以避免成为团队的瓶颈。通过参与实际项目中的代码开发，可以更好地理解团队面临的挑战 。
避免瓶颈陷阱：架构师不应过多参与关键路径的编码工作，而是应将这些任务分配给开发团队，以防止自己成为项目的瓶颈 。

ps: 没有完美架构，都是trade off





