### 第3章　体系结构：设计成功平台的原则

 #### 核心交互：平台设计的根本原因

      1、核心交互有三个关键要素：参与者 （participants）、价值单元 （valce unit）、过滤器 （filter）

###### 参与者 （participants）

- （1）核心交互的根本参与者就是两种人：创造价值的生产者和使用价值的消费者。要定义核心交互，我们需要明确地描述和理解这两种角色。

      例子：在爱彼迎上，同一个人既可能是房东，也可能是旅行者。

###### 价值单元 （valce unit）：最重要而且最难以控制的元素。

- （1）几乎每个核心交互的开端都是生产者对于价值单元的创造。

      例子：在eBay或爱彼迎上，产品与服务的信息列表都是卖家创造的价值单元，然后基于买家的搜索请求或先前表示出的兴趣为他们提供服务。

###### 过滤器 （filter）
- （1）过滤器是有着严格算法、以软件为基础的工具，平台会用它来完成用户间适当价值单元的交换。
- （2）价值单元是经过过滤器处理后传递给特定消费者的。
- （3）搜索请求就是其中一种过滤器，参与者会搜索相关词条来寻找他们感兴趣的信息。每个平台都会利用过滤器来进行信息交换。

> （考点）网络上文章所受到的赞、转发、评论以及其他回复等。--社交元素

#### 二、吸引、促进、匹配：平台设计的方式

    1、平台必须发挥三个关键功能：吸引 （pull）、促进 （faciliate）、匹配 （match）。

###### 吸引 （pull）:

    （考点）
    1、刚开始的时候，平台需要解决管道商业模式不会有的“先有鸡还是先有蛋”的问题；关于吸引的第二个问题是如何保持已注册平台用户的黏性。

    2、其中一种能够让用户反复使用平台的工具是反馈回路 （feedback loop）。有效的反馈回路可以扩大网络，提升价值，强化网络效应。

- （1）其中一种反馈回路是单用户反馈回路 （single-user feedback loop）.这是一种嵌入平台的算法，它能分析用户活动，最终得出用户的兴趣、喜好、需求，并向用户推荐其他对于他们可能存在价值的价值单元和关联。

- （2）多用户反馈回路 （multi-user feedback loop）：生产者的活动会递交给相关消费者，而消费者的活动也会给予生产者很多反馈。如果它能够有效运行，就可以创造良性循环，增加双方的活动，最终加强网络效应。Facebook的动态信息就是典型的多用户反馈回路。

- （3）其他因素也会影响平台吸引用户的能力，其中一个就是平台内现有货币的价值。

- （4）吸引力也可以通过利用外部网络的参与者来增加。

###### 促进 （faciliate）

 -（1）设定一些价值可以被创造和交换的机制，并制定原则来管理交互过程。促进过程还需要减少使用障碍。（Facebook和ins例子的对比，允许用户在一个设备上只经过三个点击操作就可以完成对图片的拍摄、修改和分享），减少使用障碍能够有助于互动的进行，并扩大参与者数量。

- （2）促进一方面是要让生产者更加方便地创造和交换商品与服务。

###### 匹配 （match）

- （1）它会利用生产者、消费者、价值单元和要交换的商品与服务的信息来完成这个目标。平台获得的信息越多，收集、组织、分类、解析数据的算法设计得越好，过滤器越精准，用来交换的信息就会越有用，生产者与消费者正确匹配得到的回报就越高。
- （2）作为设计过程的一部分，平台公司需要设计出一个明确的数据获取策略。一些平台以奖励机制鼓励参与者提供个人数据，其他平台会利用游戏元素来收集信息。（领英就设计了一个进度条来促使用户完善个人信息，渐渐地完善了其数据库。）

#### 三、在平台设计上使用端到端原则

###### 端到端原则 （end-to-end principle）

- （1）最初被萨特泽（J.H.Saltzer）、里德（D.P.Reed）和克拉克（D.D.Clark）于1981年提出。

- （2）端到端原则是指对于通用网络，专用功能应该存于末端主机而非中间节点。[](#filepos696198)[<u>6</u>](#filepos696198) 换句话说，对整个网络没用，但是对某些用户有用的功能应该被放在网络的边缘区域，远离核心区域。

- （3）端到端原则也可以被应用到平台的设计上。对于平台来说，这个原则认为专业型应用功能应该放在平台的边缘或者上层，而不是放在平台根部的最底层。

#### 四、模块化的力量

###### 模块化 （modularity）

- （1）是一种用来有效组织复杂产品和进程的战略。

- （2）模块化系统是由那些独立设计，但仍有整体功能的单位（或模块）组成。设计师通过将信息分割为可视化的设计规则和隐性的设计参数实现模块化。

- （3）使模块化奏效的一个关键因素是，当系统被清晰地地划分成子系统，它们可以通过定义明确的接口进行连接与通信，从而作为一个整体工作。这意味着，只要子系统坚持整体设计规则，且仅与系统其他部分通过标准接口连接，它们是可以被单独设计的。读者可能已经听说过应用程序接口（application programming interface，API）这个术语。

- （4）鲍德温和克拉克（1996）提出的模块化。

- （5）模块化的力量是个人计算机产业在20世纪90年代增长如此迅速的原因之一。

###### 设计结构矩阵（design structure matrics）

- （1）它能够将合成系统的依赖性进行可视化检验。

#### 五、为平台重建体系结构

- （1）将重建平台体系结构的伎俩转化为模块设计是可能的。第一步就是要分析这个系统已经被模块化的程度。

- （2）其中最关键的工具是设计结构矩阵（design structure matrics），它能够将合成系统的依赖性进行可视化检验。

- （3）2006年发表在《管理科学》杂志（Management Science）的一篇文章中，麦克拉肯（Alan MacCormack）和鲍德温记录了一个产品成功地从整体进化成模块化架构的例子。

#### 六、反复改进：反设计原则
- （1）当你正推出一个新平台或者寻求现有平台发展时，重视平台设计原则会最大限度地增加价值创造。
- （2）记住一个平台区别于传统商业的关键特质：其大多数活动都是由用户控制，而非由平台的拥有者或管理者控制。

#### 标签 （hashtag）

- （1）克里斯·梅西纳（Chris Messina），一个在谷歌工作的工程师，开始建议使用标签 （hashtag）标注和发现相似的推文.

- （2）如今，标签成了推特的中流砥柱。

> 平台设计师应该始终为偶然的发现留有余地，因为是**用户**经常指明了设计应该发展的方向。

    智能化设计:是建立和维持一个成功的平台必不可少的。但有时，最好的设计是反设计，它能为偶然、无意识甚至怪异留下空间。
###### 参与者 （participants）

- （1）核心交互的根本参与者就是两种人：创造价值的生产者和使用价值的消费者。要定义核心交互，我们需要明确地描述和理解这两种角色。

      例子：在爱彼迎上，同一个人既可能是房东，也可能是旅行者。

###### 价值单元 （valce unit）：最重要而且最难以控制的元素。

- （1）几乎每个核心交互的开端都是生产者对于价值单元的创造。

>例子：在eBay或爱彼迎上，产品与服务的信息列表都是卖家创造的价值单元，然后基于买家的搜索请求或先前表示出的兴趣为他们提供服务。

###### 过滤器 （filter）

- （1）过滤器是有着严格算法、以软件为基础的工具，平台会用它来完成用户间适当价值单元的交换。
- （2）价值单元是经过过滤器处理后传递给特定消费者的。
- （3）搜索请求就是其中一种过滤器，参与者会搜索相关词条来寻找他们感兴趣的信息。每个平台都会利用过滤器来进行信息交换。

#### 二、吸引、促进、匹配：平台设计的方式
      1、平台必须发挥三个关键功能：吸引 （pull）、促进 （faciliate）、匹配 （match）。
######  吸引 （pull）:
- 1、刚开始的时候，平台需要解决管道商业模式不会有的“先有鸡还是先有蛋”的问题；关于吸引的第二个问题是如何保持已注册平台用户的黏性。

- 2、其中一种能够让用户反复使用平台的工具是反馈回路 （feedback loop）。有效的反馈回路可以扩大网络，提升价值，强化网络效应。

- （1）其中一种反馈回路是单用户反馈回路 （single-user feedback loop）.这是一种嵌入平台的算法，它能分析用户活动，最终得出用户的兴趣、喜好、需求，并向用户推荐其他对于他们可能存在价值的价值单元和关联。

- （2）多用户反馈回路 （multi-user feedback loop）：生产者的活动会递交给相关消费者，而消费者的活动也会给予生产者很多反馈。如果它能够有效运行，就可以创造良性循环，增加双方的活动，最终加强网络效应。Facebook的动态信息就是典型的多用户反馈回路。

- （3）其他因素也会影响平台吸引用户的能力，其中一个就是平台内现有货币的价值。

- （4）吸引力也可以通过利用外部网络的参与者来增加。

###### 促进 （faciliate）

- （1）设定一些价值可以被创造和交换的机制，并制定原则来管理交互过程。促进过程还需要减少使用障碍。（Facebook和ins例子的对比，允许用户在一个设备上只经过三个点击操作就可以完成对图片的拍摄、修改和分享），减少使用障碍能够有助于互动的进行，并扩大参与者数量。

- （2）促进一方面是要让生产者更加方便地创造和交换商品与服务。

###### 匹配 （match）

- （1）它会利用生产者、消费者、价值单元和要交换的商品与服务的信息来完成这个目标。平台获得的信息越多，收集、组织、分类、解析数据的算法设计得越好，过滤器越精准，用来交换的信息就会越有用，生产者与消费者正确匹配得到的回报就越高。

- （2）作为设计过程的一部分，平台公司需要设计出一个明确的数据获取策略。一些平台以奖励机制鼓励参与者提供个人数据，其他平台会利用游戏元素来收集信息。（领英就设计了一个进度条来促使用户完善个人信息，渐渐地完善了其数据库。）

#### 三、在平台设计上使用端到端原则

###### 端到端原则 （end-to-end principle）

- （1）最初被萨特泽（J.H.Saltzer）、里德（D.P.Reed）和克拉克（D.D.Clark）于1981年提出。

- （2）端到端原则是指对于通用网络，专用功能应该存于末端主机而非中间节点。[](#filepos696198)[<u>6</u>](#filepos696198) 换句话说，对整个网络没用，但是对某些用户有用的功能应该被放在网络的边缘区域，远离核心区域。

- （3）端到端原则也可以被应用到平台的设计上。对于平台来说，这个原则认为专业型应用功能应该放在平台的边缘或者上层，而不是放在平台根部的最底层。

#### 四、模块化的力量

###### 模块化 （modularity）

- （1）是一种用来有效组织复杂产品和进程的战略。

- （2）模块化系统是由那些独立设计，但仍有整体功能的单位（或模块）组成。设计师通过将信息分割为可视化的设计规则和隐性的设计参数实现模块化。

- （3）使模块化奏效的一个关键因素是，当系统被清晰地地划分成子系统，它们可以通过定义明确的接口进行连接与通信，从而作为一个整体工作。这意味着，只要子系统坚持整体设计规则，且仅与系统其他部分通过标准接口连接，它们是可以被单独设计的。读者可能已经听说过应用程序接口（application programming interface，API）这个术语。

> （4）鲍德温和克拉克（1996）提出的模块化。

- （5）模块化的力量是个人计算机产业在20世纪90年代增长如此迅速的原因之一。

###### 设计结构矩阵（design structure matrics）

- （1）它能够将合成系统的依赖性进行可视化检验。

#### 五、为平台重建体系结构

- （1）将重建平台体系结构的伎俩转化为模块设计是可能的。第一步就是要分析这个系统已经被模块化的程度。

- （2）其中最关键的工具是设计结构矩阵（design structure matrics），它能够将合成系统的依赖性进行可视化检验。

- （3）2006年发表在《管理科学》杂志（Management Science）的一篇文章中，麦克拉肯（Alan MacCormack）和鲍德温记录了一个产品成功地从整体进化成模块化架构的例子。

##### 六、反复改进：反设计原则

- （1）当你正推出一个新平台或者寻求现有平台发展时，重视平台设计原则会最大限度地增加价值创造。

- （2）记住一个平台区别于传统商业的关键特质：其大多数活动都是由用户控制，而非由平台的拥有者或管理者控制。

###### 标签 （hashtag）

- （1）克里斯·梅西纳（Chris Messina），一个在谷歌工作的工程师，开始建议使用标签 （hashtag）标注和发现相似的推文.

- （2）如今，标签成了推特的中流砥柱。

      平台设计师应该始终为偶然的发现留有余地，因为是用户经常指明了设计应该发展的方向。

> **智能化设计**是建立和维持一个成功的平台必不可少的。但有时，最好的设计是反设计，它能为偶然、无意识甚至怪异留下空间。
