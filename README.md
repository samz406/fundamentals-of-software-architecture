# fundamentals-of-software-architecture 学习笔记

## 第一章
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


## 第二章 架构思维

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


## 第三章 模块化


##### 定义

模块化在软件架构中是一个核心概念，但其定义常常混乱且不统一。一般来说，模块化是指将相关代码逻辑分组的方法，这可以是面向对象语言中的类组，或结构化或函数式语言中的函数组​​。大多数编程语言提供了某种模块化机制，如Java中的包（package）和.NET中的命名空间（namespace）。

##### 模块化的意义

模块化是组织代码的一种原则，目的是通过逻辑分组来管理代码的复杂性。如果架构师在设计系统时不关注各个部分的相互连接方式，就会导致系统难以维护和扩展​​。模块化有助于保持系统结构的有序性和一致性，即使在项目需求中没有明确要求，也需要架构师主动确保模块间的良好区分和沟通。

##### 模块化复用

在面向对象编程之前，开发者使用模块化语言来组织代码，例如Modula和Ada。这些语言提供了类似于今天的包或命名空间的编程结构，用于逻辑分组相关代码​​。尽管面向对象语言引入了类和继承等新概念，模块化的思想仍然保留了下来。

##### 度量模块化

架构师需要工具来理解和度量模块化。关键概念包括内聚性、耦合性和共生性​​。

###### 内聚性

内聚性衡量模块内各部分的相关程度。高内聚性意味着模块的各部分紧密相关，所有部分应包含在同一模块内。例如，功能内聚的模块中，每个部分都与其他部分相关，并且模块包含完成其功能所需的一切​​。

内聚性是指模块内部各部分之间的紧密程度，它衡量的是模块内的元素在一起工作的合理性和相关性。高内聚性意味着模块内的各个元素密切相关，共同实现一个明确的功能或目标。内聚性是评估模块化设计质量的重要标准之一，因为高内聚性通常表示模块更容易理解、维护和复用。

内聚性的类型

内聚性从高到低可以分为以下几种类型：

- 功能内聚（Functional Cohesion）


定义：模块内的所有元素共同完成单一功能。

示例：一个模块负责处理用户登录验证，包括接收用户输入、验证用户名和密码、返回验证结果。

特点：这种内聚性最高，模块内的所有元素都与完成该功能密切相关，任何对功能的更改都在模块内完成。

- 顺序内聚（Sequential Cohesion）

定义：模块内的元素按顺序执行，每个元素的输出作为下一个元素的输入。

示例：一个模块首先读取文件数据，然后处理数据，最后将结果写入数据库。

特点：元素之间存在顺序依赖关系，功能较为集中，但各部分之间的联系较强。

- 通信内聚（Communicational Cohesion）


定义：模块内的元素操作同一数据集合。

示例：一个模块负责从数据库中读取数据、处理数据并生成报告。

特点：元素通过共享数据联系在一起，数据变化可能会影响多个元素。

- 过程内聚（Procedural Cohesion）

定义：模块内的元素必须按特定顺序执行，但不一定操作相同的数据。

示例：一个模块包括一系列用户界面操作步骤，如显示登录页面、接收输入、验证用户。

特点：步骤之间有顺序依赖，但数据和功能之间的关联性较低。

- 时间内聚（Temporal Cohesion）

定义：模块内的元素在同一时间段执行。

示例：一个初始化模块负责在系统启动时执行多个初始化任务，如加载配置文件、建立数据库连接。

特点：元素仅在时间上相关，功能上可能毫无关联。

- 逻辑内聚（Logical Cohesion）

定义：模块内的元素执行逻辑上相似的任务，但实际上可以独立完成。

示例：一个输入输出模块包含读取文件、读取数据库、读取网络数据等功能。

特点：元素之间逻辑相关，但彼此独立，内聚性较低。

- 偶然内聚（Coincidental Cohesion）

定义：模块内的元素没有任何明显的关系，只是偶然被放在一起。

示例：一个模块包含各种杂乱无章的功能，如日志记录、数据转换、用户通知等。

特点：这种内聚性最低，模块内的元素彼此独立，维护困难，修改时容易引入错误。

内聚性的影响

可维护性：高内聚性的模块更容易理解和修改，因为所有相关功能都集中在一起。维护高内聚性模块时，开发者可以集中关注该模块的特定功能，而不必担心其他不相关的部分。
复用性：高内聚性的模块更容易复用，因为其功能明确且独立。一个功能内聚的模块可以在不同项目或系统中被直接使用，而无需做大量修改。
测试性：高内聚性的模块更容易测试，因为其功能集中，测试覆盖率更高。测试一个高内聚性的模块通常只需要考虑模块内部的逻辑，而不必处理大量的外部依赖。
灵活性：高内聚性的模块在系统中更灵活，可以更容易地进行重构和扩展。因为其内部元素紧密相关，更改或扩展一个功能通常只影响该模块内部，而不会波及到其他模块。
实现高内聚性的方法
单一职责原则（Single Responsibility Principle, SRP）

定义：一个模块只负责一个功能或职责。
应用：确保每个模块只包含实现该功能所需的代码，避免将无关的功能混杂在一起。
模块化设计

定义：将系统划分为多个独立的模块，每个模块都有明确的职责和功能。
应用：根据功能将代码分组，确保每个模块内部的功能紧密相关，模块之间的依赖最小化。
重构

定义：通过调整代码结构来提高内聚性和降低耦合性。


###### 耦合性

耦合性衡量模块之间的相互依赖程度。较低的耦合性意味着模块间依赖较少，模块可以更独立地变化。Edward Yourdon和Larry Constantine在1979年定义了两个关键耦合性指标：传入耦合（afferent coupling）和传出耦合（efferent coupling）​​。

抽象度、稳定性和主序列距离（Abstractness, Instability, and Distance from the Main Sequence）
Robert Martin定义了一些派生度量来深入评估模块化，其中包括抽象度、稳定性和主序列距离​​。

抽象度（Abstractness）：抽象工件（如抽象类和接口）与具体工件（如实现类）的比率。
稳定性（Instability）：传出耦合与传入和传出耦合之和的比率。
公式如下：


在这些公式中，ma代表抽象元素，mc代表具体元素，Ce代表传出耦合，Ca代表传入耦合。主序列距离（Distance from the Main Sequence）衡量抽象度与稳定性之间的理想关系，类的位置越接近理想线，类的平衡性越好​​。

###### 共生性

Meilir Page-Jones在1996年提出了共生性的概念，用于描述软件系统中两个组件之间的依赖关系。**当一个组件的变化需要另一个组件也做出相应变化以保持系统的正确性时，这两个组件被称为共生性​​**。

共生性分为两种类型：

静态共生性: 

  是指源代码级的耦合，它是对Structured Design中定义的传入耦合和传出耦合的细化，架构师将以下静态共生性的类型视作事物之间相互耦合的程度，无论它们是传入耦合还是传出耦合：包含如下类型：

- 名称共生性

定义：多个组件必须使用相同的名称来引用某个实体。
示例：方法名是代码库中最常见的耦合方式，尤其是在现代重构工具可以轻松地进行系统范围内的名称更改时​​。

- 类型共生性

定义：多个组件必须同意实体的类型。
示例：这类共生性在许多静态类型语言中很常见，通过类型检查来限制变量和参数的类型​​。
意义共生性

定义：多个组件必须同意特定值的意义。
示例：代码库中硬编码的数值是最常见的例子，如定义 int TRUE = 1; int FALSE = 0;​​。
位置共生性

定义：多个组件必须同意值的顺序。
示例：方法和函数调用中的参数值顺序问题​​。

算法共生性

定义：多个组件必须同意使用特定的算法。
示例：安全哈希算法必须在服务器和客户端上生成相同的结果以进行用户验证​​。

动态共生性: 分析运行时调用


- 执行顺序共生性

定义：多个组件的执行顺序是重要的。

示例：电子邮件发送顺序：必须先设置收件人和发件人，然后才能发送邮件​​。

- 时间共生性

定义：多个组件的执行时间是重要的。

示例：两个线程同时执行可能会导致竞态条件，从而影响联合操作的结果​​。

- 值共生性

定义：多个值之间存在依赖关系，必须一起更改。

示例：分布式系统中的事务处理，所有值必须一起更改，否则不能更改​​。

- 身份共生性

定义：多个组件必须引用相同的实体。

示例：独立组件共享和更新公共数据结构，如分布式队列​​


###### 共生性的属性

强度（Strength）：强度决定了重构的难易程度。架构师应优先考虑强度较低的共生性，因为它们更容易重构​​。
局部性（Locality）：共生性的局部性衡量模块之间的接近程度。同一模块内的强共生性比跨模块的强共生性对代码库的影响更小​​。
程度（Degree）：共生性的程度与其影响范围有关。影响范围较小的共生性对代码库的破坏较小​​。
Jim Weirich提出了两条关于共生性的重要建议：

程度规则：将强共生性转换为弱共生性。

局部性规则：随着软件元素之间距离的增加，使用更弱的共生性形式​​。

Page-Jones提供了三种通过共生性来提升系统模块化的准则:

1.将系统分解为封装元素来最小化整体共生性

2.最小化跨越封装边界的任何剩余共生性

3.最大化封装边界内的共生性


###### 统一耦合和共生性指标
<img width="712" alt="image" src="https://github.com/user-attachments/assets/90967ddb-0542-4e18-ab6a-ff2ab39eee0f">


##### 从模块到组件

架构师通常从组件的角度来思考系统。组件是模块的物理实现形式，开发者可以以不同的方式打包组件，具体取决于其开发平台。例如，Java中的jar文件、.NET中的dll文件等​​。

组件构成了架构中的基本模块化构建块，是架构师必须关注的关键内容之一。架构师的主要任务之一是确定组件的顶级划分​​。



## 第四章 架构特性定义


### 架构特性的定义标准

一个架构特性需要满足以下三个标准：

非领域设计考虑因素：架构特性描述了如何实现系统需求及其原因，而不仅仅是系统应做什么。例如，性能通常不会出现在需求文档中，但它是一个重要的架构特性 。

影响设计的某些结构方面：架构特性往往需要特定的结构考虑。例如，安全性是大多数项目的关注点，如果系统需要处理支付处理，架构可能需要设计一个特定的模块来处理这些敏感信息 。

对应用成功至关重要：支持每个架构特性会增加设计的复杂性，因此架构师需要选择最少的架构特性，而不是尽可能多 。

### 架构特性的分类

#### 操作性架构特性

操作性架构特性涵盖了系统在运行时必须具备的能力，如性能、可扩展性、弹性、可用性和可靠性。以下是一些常见的操作性架构特性 ：

可用性：系统需要多长时间可用。

连续性：灾难恢复能力。

性能：包括压力测试、峰值分析、功能使用频率分析、所需容量和响应时间。

可恢复性：灾难发生后系统需要多快恢复在线。

可靠性/安全性（Reliability/Safety）：评估系统是否需要故障安全或任务关键。

鲁棒性（Robustness）：在运行过程中处理错误和边界条件的能力。

可扩展性（Scalability）：系统在用户数量或请求增加时的性能和操作能力。

#### 结构性架构特性

结构性架构特性关注代码结构和质量，如良好的模块化、受控的组件之间的耦合、可读代码等。以下是一些常见的结构性架构特性 ：

可配置性（Configurability）：终端用户通过可用界面轻松更改软件配置的能力。

可扩展性（Extensibility）：添加新功能的难易程度。

可安装性（Installability）：系统在所有必要平台上的安装难易程度。

杠杆性/复用性（Leverageability/Reuse）：在多个产品中复用通用组件的能力。

本地化（Localization）：支持多语言输入/查询屏幕、数据字段、报告等。

可维护性（Maintainability）：应用更改和增强系统的难易程度。

可移植性（Portability）：系统是否需要在多个平台上运行。

支持性（Supportability）：应用所需的技术支持级别。

可升级性（Upgradeability）：从旧版本升级到新版本的难易程度。

#### 跨领域架构特性（Cross-Cutting Architecture Characteristics）

某些架构特性难以归类，但它们仍然是重要的设计约束和考虑因素。以下是一些常见的跨领域架构特性 ：

可访问性（Accessibility）：包括色盲、听力障碍等残疾用户的访问。

可归档性（Archivability）：数据是否需要归档或在一段时间后删除。

认证（Authentication）：确保用户身份的安全要求。

授权（Authorization）：确保用户只能访问应用的某些功能的安全要求。

法律合规性：系统运营中涉及的立法约束。

隐私：对内部公司员工隐藏事务的能力。

安全性：数据在数据库中的加密需求、内部系统之间网络通信的加密需求等。

可支持性：应用所需的技术支持级别和调试系统错误所需的日志记录设施。

可用性/可达成性：用户通过应用达到目标所需的培训级别。

#### 架构特性之间的权衡

应用程序通常只能支持我们列出的少数几个架构特性，原因多种多样。首先，每一个支持的特性都需要设计上的努力，甚至可能需要结构上的支持。其次，更大的问题在于，每个架构特性往往会影响到其他特性。例如，如果架构师想要提高安全性，几乎肯定会对性能产生负面影响：应用程序必须进行更多的实时加密、秘密隐藏的间接处理以及其他可能降低性能的活动。

一个比喻可以帮助说明这种互联性。据说飞行员在学习驾驶直升机时经常会遇到困难，因为驾驶直升机需要每只手和每只脚都控制一个操纵杆，改变一个操纵杆会影响到其他操纵杆。因此，驾驶直升机是一种平衡的练习，这很好地描述了选择架构特性时的权衡过程。每个架构师设计支持的架构特性都有可能使整体设计变得复杂。

因此，架构师很少遇到能够设计一个系统并最大化每个架构特性的情况。更多的时候，**决策是几种相互竞争的关注点之间的权衡**

#### 设计“最不差”架构

总之，架构师很少能设计出在每个方面都最佳的系统。通常，决策涉及多个相互竞争的关注点之间的权衡 。架构师应尽量设计可迭代的架构，这样可以更容易地对架构进行更改，从而减少复杂性和风险 。


## 第五章：识别架构特性


识别关键的架构特性是创建架构或确定现有架构有效性的重要步骤。要识别适用于特定问题或应用的正确架构特性（“-ilities”），架构师不仅需要了解领域问题，还需要与问题域的利益相关者合作，以确定从领域角度看什么是真正重要的 。

### 从领域关注点中提取架构特性

架构师必须能够将领域关注点转化为架构特性。例如，扩展性是最重要的关注点，还是容错性、安全性或性能？也许系统需要所有这四个特性。了解关键的领域目标和领域情况可以让架构师将这些领域关注点转化为“-ilities”，从而形成正确且合理的架构决策的基础 。

在与领域利益相关者合作定义驱动架构特性时，一个提示是尽量保持最终列表尽可能简短。架构中的一个常见反模式是试图设计一个通用架构，支持所有架构特性。每个支持的架构特性都会增加系统设计的复杂性；支持太多的架构特性会在架构师和开发人员还没有开始解决问题域时就导致复杂性大大增加。因此，不要过分关注特性的数量，而要关注保持设计简单的动机 。

案例研究：Vasa战舰

Vasa战舰是过度规定架构特性最终导致项目失败的经典例子。这是一艘瑞典战舰，建造于1626年至1628年间，由希望建造最宏伟战舰的国王下令建造。当时的船只通常是运兵船或战舰，而Vasa战舰要同时具备这两种功能。大多数船只有一层甲板，而Vasa战舰有两层！尽管经验丰富的造船工匠有些担忧，但最终还是完成了建造。在庆祝时，战舰驶入港口并向一侧发射了炮弹。由于战舰重心过高，最终倾覆并沉入瑞典湾底。这个故事告诉我们，过度规定架构特性会导致设计复杂性和风险增加，最终可能导致项目失败 。

### 从需求中提取架构特性


#### 从需求中提取架构特性

从需求中提取架构特性需要架构师深入理解需求文档并识别出其中的架构特性。架构师必须将需求翻译成架构特性，以确保系统满足这些需求。例如，一个购物网站可能希望支持特定数量的并发用户，这是需求文档中明确规定的。架构师需要将这种需求转化为扩展性特性，以确保系统能够处理大量并发用户而不会出现性能问题 。

#### 隐含特性

隐含特性是指那些没有明确写在需求文档中的特性，但它们对系统的成功至关重要。例如，安全性可能不会在需求文档中明确指出，但对于处理支付信息的系统来说，安全性是不可或缺的 。

案例研究：硅三明治（Silicon Sandwiches）

为了更好地说明这些概念，书中引入了一个架构Kata——硅三明治（Silicon Sandwiches）。这个案例研究展示了架构师如何从需求中提取架构特性 。

描述：一家全国性的三明治店希望实现在线订购（除了现有的电话订购服务）。

用户：成千上万，可能有一天会有数百万用户。

需求：

用户下订单后，将获得一个取餐时间和商店的方向（需要集成多个外部地图服务，包括交通信息）。

如果商店提供送餐服务，调度司机将三明治送到用户手中。

移动设备可访问性。

提供全国每日促销/特价。

提供本地每日促销/特价。

接受在线支付、现场支付或送餐支付 。

附加背景：

三明治店是特许经营店，每家店都有不同的店主。
总公司计划在不久的将来扩展到海外。
公司目标是雇佣廉价劳动力以最大化利润 。
在这个场景中，架构师如何提取架构特性呢？架构师不会在这里设计整个系统，而是寻找那些影响或影响设计的因素，特别是结构性的因素 。

#### 显式特性

显式架构特性出现在需求规范中，作为必要设计的一部分。例如，一个购物网站可能希望支持特定数量的并发用户，这在需求规范中由领域分析师指定。架构师需要考虑需求的每一部分，看看它是否构成架构特性 。

一个架构师首先应该注意到的细节是用户数量：目前是成千上万，可能有一天会达到数百万。因此，扩展性——处理大量并发用户而不会严重性能下降的能力——是顶级架构特性之一。注意，这个问题陈述并没有明确要求扩展性，而是以预期用户数量的形式表达了这一需求。架构师经常需要将领域语言解码为工程等价物 。



