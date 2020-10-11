# One-man-one-month-myth 人月神话

## The Tar Pit 焦油坑

- 程序 -> 编程产品，编程系统 -> 编程系统产品
- 编程的快乐
  - 创建事物的纯粹快乐
  - 快乐来自于开发对其他人有用的东西
  - 整个过程体现出魔术般的力量——将互相啮合的零部件组装在一起
  - 学习的乐趣
  - 乐趣还来自于工作在如此易于驾驭的介质上
- 编程的苦恼
  - 必须追求完美（将做事的方式往追求完美的方向调整）
  - 是由他人来设定目标，供给资源，提供信息
  - 概念性设计是有趣的，但是寻找琐碎的bug却是一项重复性的活动
  - 当投入了大量辛苦的劳动，产品在即将完成或者终于完成的时候，却已显得陈旧过时
- 编程，一个许多人痛苦挣扎的焦油坑以及一种乐趣和苦恼共存的创造性活动。

## The Mythical Man-Month 人月神话

- 缺乏合理的时间进度是造成项目滞后的最主要原因
  - 对估算技术缺乏有效的研究（不真实的假设——一切将运作良好）
  - 采用的估算技术隐含地假设人和月可互换，错误地将进度与工作量互相混淆
  - 由于对自己的估算缺乏信心，软件经理通常不会有耐心地持续进行估算这项工作
  - 对进度缺少跟踪和监督
  - 当意识到进度的偏移时，下意识的反应是增加人力（火上浇油）
- 乐观主义
  - 系统编程进度安排背后的第一个假设：一切将运作良好，每一项任务仅花费他所“应该”花费的时间。
  - 创造性活动：构思、实现、交流
  - 计算机编程基于十分容易掌握的介质，编程人员通过非常纯粹的思维活动——概念以及灵活的表现形式来开发程序。由于介质的易于驾驭，我们期待在实现过程中不会碰到困难，因此造成了乐观主义的弥漫。
  - 大型的编程工作，包含很多任务，任务包含前后次序，一切正常的概率非常小
- 人月
  - 第二个谬误：估计和进度安排中使用的工作量单位：人月
  - 使用人月作为衡量一项工作的规模是一个危险的带有欺骗性的神话，它暗示人员数量和时间是可以相互替换的。
  - 当任务由于次序上的限制不能分解时，人手的添加对进度没有帮助
  - 对于可以分解，但子任务之间需要相互沟通和交流的任务，必须在计划工作中考虑沟通的工作量
  - 因为软件开发本质上是一项系统工作——错综复杂关系下的一种实践——沟通、交流的工作量非常大，它很快会消耗任务分解所节省下来的个人时间。从而添加更多的人手，实际上是延长了时间进度
- 系统测试
  - 在早期进度策划时，允许充分的系统测试时间是非常重要的
- 空泛的估算
  - 为了满足顾客期望的日期而造成的不合理进度安排
  - 非阶段化方法的采用，少的可怜的数据支持，加上完全借助软件经理的知觉，很难生产出及健壮可靠和规避风险的估计
  - 解决方案1：开发并推行生产率图标、缺陷率、估算规则等，整个组织从数据的共享上获益
  - 解决方案2：在基于可靠基础的估算出现之前，项目经理需要挺直腰杆，坚持他们的估计，确信自己的经验和直觉比从期望派生出的结果要强得多
- 重复产生的进度灾难
  - 重现“灾难”所开发出的产品，比没有增加人手，而是重新安排开发进度所产生的的产品更差
  - Brooks法则：向进度落后的项目中增加人手，只会使进度更加落后
- 除去神话色彩的人月
  - 项目的时间依赖于顺序上的限制，人员的数量依赖于单个子任务的数量

## The Surgical Team 外科手术队伍

- 研究表明，效率高和效率低的实施者之间具体差别非常大，经常达到了数量级的水平
- 进退两难的问题：对于效率和概念的完整性来说，最好由少数干练的人员来设计和开发，而对于大型系统，则需要大量的人手，以使产品能在时间上满足要求
- Mills的建议
  - 大型项目的每一个部分由一个团队解决，但队伍以类似外科手术的方式组建，由一个人来进行问题的分解，其他人给与他所需要的支持以提高效率和生产力。
  - 从个人艺术到公共实践，所有的程序和数据看作是团队所有物
  - 外科医生——首席程序员
    - 亲自定义功能和性能说明书，设计程序，编制源代码，测试以及书写技术文档
    - 天分，经验，大量知识
  - 副手
    - 外科医生的后备，具有较少的经验
    - 主要作用是作为设计的思考者、讨论者和评估人员
  - 管理员
    - 控制财务、人员、工作地点安排和机器的专业管理人员
  - 编辑
    - 根据外科医生的草稿或者口述的手稿，进行分析和重新组织，提供各种参考信息和书目，对多个版本进行维护以及监督文档生成的机制
  - 秘书
    - 管理员和编辑各需要一个秘书
  - 程序职员
    - 维护编程产品库中所有团队的技术记录
  - 工具维护人员
    - 保证所有基本服务的可靠性，以及承担团队成员所需要的特殊工具的构建、维护和升级责任
  - 测试人员
  - 语言专家
    - 寻找一种简洁有效的使用语言的方法来解决复杂、晦涩或者棘手的问题
- 如何运作
  - 十个人，七个专业人士在解决问题，而系统是一个人或者最多两个人思考的产物，客观上达到了概念的一致性
- 团队的扩建
  - 扩建过程的成功依赖于，每个部分的概念完整性得到了彻底的提高
  - 对于协调的问题，还是需要使用分解的技术。整个系统必须具备概念上的完整性，要有一个系统结构师从上至下地进行所有的设计。要使工作易于管理，必须清晰的划分体系结构设计和实现之间界限。

## Aristocracy, Democracy, and System Design 贵族专制、民主政治和系统设计

- 概念一致性
  - 在系统设计中，概念完整性应该是最重要的考虑因素。为了反映一系列连贯的设计思路，宁可省略一些不规则的特性和改进，也不提倡独立和无法整合的系统，哪怕它们其实包含着许多很好的设计
- 获得概念的完整性
  - 对于给定级别的功能，能用最简洁和直接的方式来指明事情的系统是最好的。
  - 易用性实际上需要设计的一致性和概念上的完整性
- 贵族专制统治和民主政治
  - 非常大型的项目，将设计方法、体系结构方面的工作与具体实现相分离是获得概念完整性的强有力方法
  - 系统的概念完整性决定了使用的容易程度，必须控制这些概念
  - 产品的成本性能很大程度上依靠实现人员，就如易用性很大程度上依赖结构师一样
  - 外部的体系结构规定实际上是增强，而不是限制实现小组的创造性
- 在等待时，实现人员应该做什么
  - 整个创造性活动包括了三个独立的阶段：体系结构(architecture)、设计实现(implementation)、物理实现(realization)。它们往往可以同时开始和并发执行
  - 概念的完整性的确要求系统只反映唯一的设计理念，用户所见的技术说明来自少数人的思想，实际工作被划分为3块，但这不意味着该开发模式下的系统需要更长的时间来创建。经验显示恰恰相反，整个系统将会开发得更快，所需要的测试时间更少。同工作的水平分割相比，垂直划分从根本上大大减少了劳动量，结果是使交流彻底地简化，概念完整性得到大幅提高

## The Second-System Effect 画蛇添足

- 有什么样的准则和机制来约束结构师的创造性热情：结构师和建筑人员之间彻底、仔细和谐的交流

- 结构师的交互准则和机制
  - 牢记是开发人员承担创造性和发明性的实现责任，所以结构师只能建议，而不能支配
  - 时刻准备着为所指定的说明建议一种实现的方法，同样准备接受其他任何能达到目标的方法
  - 对上述的建议保持低调和冷静
  - 准备放弃坚持所作的改进建议
- 自律——开发第二个系统所带来的后果
  - 开发第二个系统引起的后果与纯粹的功能修饰和增强明显不同，也就是说存在对某些技术进行细化/精练的趋势。由于基本系统设想发生了变化，这些技术已经显得落后。
  - 结构师如何避免画蛇添足？他无法跳过二次系统，但是他可以有意识关注那些系统的特殊危险，运用特别的自我约束准则，来避免那些概念上的修饰，根据系统基本理念及目的的变更，舍弃一些功能
  - 项目经理如何避免画蛇添足？他必须坚持至少拥有两个系统以上开发经验结构师的决定。同时保持对特殊诱惑的警觉，他可以不断提出正确的问题，确保原则上的概念和目标再详细设计中得到完整的体现

## Passing the Word 贯彻执行

- 文档化的规格说明——手册
  - 手册不但要描述包括所有界面在内的用户可见的一切，它同时还要避免描述用户看不见的事物
- 形式化定义
  - 形式化的定义是精确的，它们更倾向于更加完整；差异得更加明显，可以更快地完成。但是形式化的缺点是不易理解。形式化需要记叙性文字的辅助，才能使内容易于领会和讲授
  - 形式化定义可以是一种设计实现，反之，设计实现也可以作为一种形式化定义的方法
  - 实现作为定义，通过定义所得到的答案，总是同所要求的一样精确和正确，但是实现可能更加过度地规定了外部功能
- 直接整合（？）
  - 设计被传递参数和共享存储器的声明
- 会议和大会
- 多重实现
  - 如实遵从手册更新机器所造成的延迟和成本的消耗，比根据机器调整手册要低
- 电话日志
- 产品测试

## Why Did the Tower of Babel Fail? 为什么巴比伦塔会失败？

- 巴比伦塔的管理教训
  - 项目的先决条件：清晰的目标、人力、材料、足够的时间、足够的技术
  - 交流、交流的结果——组织
- 大型编程项目中的交流
  - 非正式途径（电话）
  - 会议
  - 工作手册
- 项目工作手册
  - 是什么：对项目必须产出的一系列文档进行组织的一种结构
  - 为什么：技术说明必不可少；控制信息发布
  - 处理机制：实时更新；微缩胶片
  - 现在如何入手：采用直接访问的文件；改变的是分发机制和查询方法
- 大型编程项目的组织架构
  - 团队组织的目的是减少不必要的交流和合作的数量
  - 人力划分(division of labor)、限定职责范围(specialization of function)：树状的管理结构，网状的交流结构
  - 树状的编程队伍的每颗子树：任务、产品负责人、技术主管和结构师、进度、人力的划分、各部分之间的接口定义
    - 产品负责人和技术主管是同一个人（适用很小型团队）
    - 产品负责人作为总指挥，技术主管充当其左右手（项目经理可以使用并不很擅长管理的技术天才来完成工作）
    - 技术主管作为总指挥，产品负责人充当其左右手（适用小型团队）
- 交流和交流的结果——组织，是成功的关键。交流和组织的技能需要管理者仔细考虑，相关经验的累积和能力的提高同软件技术本身一样重要

## Calling the Shot 胸有成竹

- 工作量 = (常数) * (指令的数量)^1.5
- Portman的数据：项目估算对每个人年的技术工作时间数量做出了不现实的假设
- Aron的数据
- Harr的数据
- OS/360的数据：生产率会根据任务本身复杂度和困难程度表现出显著的差异
- Corbato的数据
  - 对常用编程语句而言，生产率似乎是固定的。这个生产率包括了编程中需要注释，并可能存在错误的情况
  - 使用适当的高级语言，编程的生产率可以提高5倍

## Ten Pounds in a Five-Pound Sack 削足适履

- 作为成本的程序空间
  - 开发人员必须设置规模的目标，控制规模，考虑减小规模的方法
- 规模控制
  - 仅对核心程序设定规模目标是不够的，必须把所有的方面都编入预算：和制订驻留空间预算一样，应该制订总体规模的预算；和制订规模预算一样，应该制订后台存储访问的预算
  - 在指明模块有多大的同时，确切定义模块的功能
  - 从系统整体出发，面向用户的态度是软件编程人员最重要的职能
- 空间技能
  - 速度不变，以功能换尺寸。设计人员必须决定用户可选项目的粗细程度
  - 内存一定，考虑空间-时间的折衷
    - 确保团队在编程技能上得到培训，而不仅仅是依赖他们自己掌握的知识和先前的经验
    - 认识到编程需要技术积累，需要开发很多公共单元构件
- 数据的表现形式是编程的根本

## The Documentary Hypothesis 提纲挈领

- 文档的跟踪维护是项目监督和预警的机制，文档本身可以作为检查列表、状态控制，也可以作为汇报的数据基础
- 计算机产品的文档
  - 目标
  - 技术说明
  - 进度、时间表
  - 预算
  - 组织机构图
  - 工作空间的分配
  - 报价、预测、价格
- 大学科系的文档(...)
- 软件项目的文档
  - 做什么：目标
  - 做什么：产品技术说明
  - 时间：进度表
  - 资金：预算
  - 地点：工作空间分配
  - 人员：组织图
- 为什么要有正式的文档
  - 书面记录决策是必要的
  - 文档能够作为同其他人的沟通渠道
  - 项目经理的文档可以作为数据基础和检查列表

## Plan to Throw One Away 未雨绸缪

- 试验性工厂和增大规模
  - 原型
  - 为舍弃而计划
- 唯一不变的就是变化本身
  - 变化时与生俱来的，不是不合时宜和令人生厌的异常情况
  - 抛弃原型概念本身就是对事实的接受——随着学习的过程更改设计
- 为变更计划系统
  - 高级语言和自文档技术
  - 变更的阶段化是一种必要的技术
- 为变更计划组织结构
  - 组建外科手术式的软件开发团队，最小化成员间的接口，一个长期有效的灵活组织架构解决方案
- 前进两步，后退一步
  - 软件维护中，缺陷修复总会以(20% - 50%)的几率引入新的bug
  - 看上去很轻微的错误实际上是系统级别的问题
  - 作为引入新bug的一个后果，程序每条语句的维护需要的系统测试比其他编程要多
  - 显然，使用能消除、至少是能指明副作用的程序设计方法，会在维护成本上有很大的回报
- 前进一步，后退一步
  - 模块数量随版本号的增长呈线性增长，但是受到影响的模块以版本号指数的级别增长。所有修改都倾向于破坏系统的架构，增加了系统的混乱程度。随着时间的推移，系统变得越来越无序
  - 系统软件开发是减少混乱度的过程，所以它本身是处于亚稳态的

## Sharp Tools 干将莫邪

- 个性化的工具妨碍沟通，工具的生命周期是很短的，开发和维护公共的通用编程工具的效率更高
  - 计算机设施、操作系统、语言、实用程序、调试辅助程序、测试用例生成工具、文档的字处理系统
- 目标机器
  - 计划安排
- 辅助机器和数据服务
  - 仿真装置，可靠的调试平台
  - 编译器和汇编平台
  - 程序库和管理
  - 编程工具
  - 文档系统
  - 性能仿真装置
- 高级语言和交互式编程
  - 使用高级语言的主要原因是生产率和调试速度
  - 交互式编程

## The Whole and the Parts 整体部分

- 剔除bug的设计
  - 防范bug的定义
  - 测试规格说明
  - 自顶向下的设计
  - 结构化编程
    - 把系统的结构作为控制结构来考虑，而不是独立的跳转语句
- 构件单元测试
  - 本机调试
  - 内存转储
  - 快照
  - 交互式调试
  - 测试用例
- 系统集成测试
  - 使用经过调试的构件单元
    - 文档化的bug：申明构件单元的所有缺陷已经被发现，还没有被修复，但是已经做好了系统调试的准备
  - 搭建充分的测试平台
    - 供调试所用的所有程序和数据
    - 伪构件(dummy component)：仅仅由接口和可能的伪数据或者一些小的测试用例组成
    - 微缩文件(miniature file)：创建一个仅包含典型记录但涵盖全部描述的小型文件是非常值得的
    - 辅助程序(auxiliary program)：用来测试数据发生器、特殊的打印输出、交叉引用表分析
  - 控制变更
    - 有人控制和负责各个构件单元的变更或版本之间的替换
    - 必须存在系统的受控拷贝：测试版本、最终锁定版本、安全版本
    - 变更文档化
  - 一次添加一个构件
  - 阶段（量子）化、定期变更
    - 直到下一次系统构建的定期发布之前，都一直使用快速补丁
    - 在当前的发布中，把已经用过测试并进行了文档化的修补措施整合到系统平台

## Hatching a Catastrophe 祸起萧墙

- 里程碑还是沉重的负担？
  - 里程碑的选择只有一个原则：必须是具体的、特定的、可度量的时间，能够进行清晰定义。
    - 里程碑是百分之百的事件
- “其他的部分反正会落后”
  - 进取，进取提供了缓冲和储备，使开发队伍能够处理常规的异常事件，可以预计和防止小的灾祸
  - PERT图，展示某人为了使自己的工作原理关键路径，需要提前多少，也建议了补偿其他部分失去的时间的方法
- 地毯的下面
  - 老板需要两种信息：需要采取行动的计划方面的问题，用来进行分析的状态数据
  - 一线经理的利益与老板冲突，只要他觉得自己可以独立解决的问题就不会告诉老板
  - 掀开地毯
    - 减少角色的冲突
      - 老板必须区别行动信息和状态信息
      - 把会见、评审、会议明显标记为状态检查和问题-行动会议
      - 相应控制自己的行为
    - 猛地拉开地毯
      - 以PERT图以及频繁的里程碑为基础的，拥有了解状态真相的评审机制
      - 关键的文档
      - 计划和控制小组
- 对计划和职能控制进行适度的技术人力投资是非常值得赞赏的

## The other face 另外一面

- 文档的重要：对软件编程产品来说，程序向用户所呈现的面貌和提供给机器识别的内容同样重要
- 需要什么样的文档
  - 使用程序：目的、环境、范围、实现功能和使用的算法、输入输出格式、操作指令、选项、运行时间、精度和校验
  - 验证程序：测试用例
    - 针对遇到的大多数常规数据和程序主要功能进行测试的用例
    - 数量相对较少的合法数据测试用例，对输入数据范围边界检查
    - 数量相对较少的非法数据测试用例，在边界外检查数据范围边界
  - 修改程序
    - 流程图或子系统的结构图
    - 对所用算法的完整描述
    - 对所有文件规划的解释
    - 数据流的概要描述
    - 初始设计中预见修改的讨论；特性、功能回调的位置以及出口；原作者对可能扩充的地方以及可能处理方案的一些意见
- 流程图
  - 一页纸
- 自文档化(self-documenting)的程序
  - 合并文件，把文档整合到源代码
  - 方法
    - 借助那些出于语言的要求而必须存在的语句，来附加尽可能多的“文档”信息
    - 尽可能使用空格和一致的格式提高程序的可读性，表现从属和嵌套关系
    - 以段落注释的形式，向程序中插入必要的记叙性文字
  - 一些技巧
    - 为每次运算使用单独的任务名称
    - 使用包含版本号和能帮助记忆的程序名称
    - 在过程的注释中，包含记叙性的描述文字
    - 尽可能为基本算法提供参考引用，通常它会指向更完备的处理方法
    - 显示和算法书籍中的传统算法的关系
    - 声明所有的变量
    - 用标签标记初始化的位置
    - 对程序语句进行分组和标记，以显示与设计文档中语句单元的一致性
    - 利用缩进表现结构和分组
    - 在程序列表中，手工添加逻辑箭头
    - 使用行注释来解释任何不很清楚的事情
    - 把多条语句放置在一行，或者把一条语句拆放在若干行，以吻合逻辑思维
  - 为什么不
    - 必须存储的源代码规模的增加
  - 自文档化的方法激发了高级语言的使用，特别是用于在线系统的高级语言

---

> 额外收录的没有银弹、再论银弹

## No Silver Bullet —— Essence and Accient in Software Engineering 没有银弹——软件工程中的根本和次要问题

> 没有任何技术或管理上的进展，能够独立地许诺十年内使生产率、可靠性或简洁性获得数量级上的进步

### 绪论

- 所有软件活动包括根本任务——打造由抽象软件实体构成的复杂概念结构，次要任务——使用编程语言表达这些抽象实体，在空间和时间限制内将它们映射成机器语言。
- 除非占了所有工作的9/10，否则即使全部次要任务的时间缩减到0，也不会给生产率带来数量级上的提高
- 需要关注软件任务中的必要活动
  - 仔细地进行市场调研，避免开发已上市的产品
  - 在获取和制订软件需求时，将快速原型开发作为迭代计划的一部分
  - 有机地更新软件，随着系统的运行、使用和测试，逐渐添加越来越多的功能
  - 不断挑选和培养杰出的概念设计人员

### 介绍

- 没有银弹
- 出现了令人振奋的一些革新，在将来使生产率产生数量级上的提高
- 进步是逐步取得的，伴随着辛勤的劳动，对规范化过程应进行持续不懈的努力。由此，诞生了现在的软件工程

### 是否一定那么困难呢？——根本困难

- 软件开发中困难的部分是规格化、设计和测试这些概念上的结构，而不是对概念进行表达和对现实逼真程度进行验证
- 现代软件系统中无法规避的内在特性
  - 复杂度
    - 规模上的复杂
    - 软件实体的扩展也不仅仅是相同元素重复添加，而必须是不同元素实体的添加
    - 软件的复杂度是必要属性
    - 复杂度不仅仅导致技术上的困难，还引发了很多管理上的问题
  - 一致性
    - 很多复杂性来自保持与其他接口的一致，对软件的任何再设计，都无法简化这些复杂特性
  - 可变性
    - 软件产品扎根于文化的母体中，母体持续不断地变化中，这些变化无情地强迫着软件随之变化
  - 不可见性
    - 不可见，无法可视化
    - 软件的客观存在不具有空间的形体特征，没有已有的表达方式
  
### 以往解决次要困难的一些突破

- 高级语言
  - 减轻了一些次要的软件复杂度
  - 可靠性、简洁性和理解程度大为提高
  - 但有可能增加了脑力劳动上的负担
- 分时
  - 保证了及时性，让我们能维持对复杂程度一个总体的把握
- 统一编程环境

### 银弹的希望

- Ada和其他高级编程语言
- 面向对象编程
  - 抽象数据类型
  - 层次化类型
- 人工智能
- 专家系统
- “自动”编程
- 图形化编程
- 程序验证
- 环境和工具
- 工作站

### 针对概念上根本问题的颇具前途的方法

- 考虑解决软件上必要困难的活动，即准确地表达复杂概念结构
- 购买和自行开发
- 需求精炼和快速原型
- 增量开发——增长，而非搭建系统
- 卓越的设计人员



## "No Silver Bullet" Refired 再论《没有银弹》

### 人狼和其他恐怖传说

### 存在着银弹——就在这里

### 含糊的表达将会导致误解

- 次要(Accidental)：软件开发中的实现过程
- 现实问题：整个软件开发工作中的哪些部分与概念性结构的精确和有序表达相关，哪些部分是创造那些结构的思维活动
- 因为是根本困难所以没有希望？
  - 每一种困难产生的麻烦都是可以改善的，例如重用和交互的构件开发
- 复杂性是层次化的
  - 系统复杂性是无数细节的函数，这些细节必须精确详细地说明
  - 在更高的级别开发软件，使用他人的成果，或者重用自己的程序——都能避免面对整个层次的复杂性
  - 层次化，通过分层的模块或者对象
  - 增量化，从而系统可以持续地运行

### Harel的分析

- 悲观主义 vs. 乐观主义 vs. 现实主义
  - 白日梦限制了向前的发展，浪费了精力
- “消极”主题
  - 根本和次要问题的清晰划分
  - 独立评价每个候选银弹
  - 仅仅预言了十年，而不是足够长的时间“出现任何重大的进步”
- 想象的试验
- 银弹就在这里
  - 香草框架
- 不可见性
  - 适当使用可视化图形可以给工程师和程序员带来可观的成效

### Jone的观点——质量带来生产率

- 关注质量，生产率自然会提高
- 一味追求质量，生产率会再次下降
- 系统化软件开发方法的发展是为了解决质量问题，而不是出于生产率方面的考虑

### 那么，生产率的情形如何？

- 生产率数据
- 塑料薄膜包装的成品软件——购买，而非开发
- 创造性活动的强大工具

### 面向对象编程——这颗铜制子弹可以吗？

- 使用更大的零件来构建
- 面向对象技术为什么发展缓慢？
  - OO程序员关注低层次而不是高层次的抽象 -> 自顶向下的设计
  - 人们将OO看作工具而不是设计的方法
- 资金的先行投入，收益的后期获得

### 重用的情况怎么样？

- 程序员经常重用他们自己手头的工作
- 现在公司级别的重用情况如何？
  - 重用是一件说起来容易，做起来难的事情，它同时需要良好的设计和文档
  - 时间证明了使模块能够重用的成本非常高

### 学习大量的词汇——对软件重用的一个可预见，但还没有被预言的问题

- 思索的层次越高，所需要处理的基本思考要素也就越多。高级语言有更广泛的词汇量、更复杂的语法以及更加丰富的语义
- 一些经验教训
  - 人们在上下文中学习，所以我们需要出版一些复合产品的例子，而不仅仅是零部件的库
  - 人们只会记忆背诵单词。语法和语义是在上下文中，通过使用逐渐地学习
  - 人们根据语义上的分类对词汇组合规则进行分组，而不是通过比较对象子集

### 子弹的本质——形势没有发生改变

- 软件开发是一件棘手的事情，前方并不会有魔术般的解决方案。
- 现在是从业者研究和分析革命性进展的时刻，而不是等待或希望它的出现
- 我们可以在软件生产率上取得逐步的进展，而不是等待不大可能到来的突破

---

## Propositions of the Mythical Man-Month: True or False 《人月神话》的观点：是或非？

...

---

## The Mythical Man-Month after 20 Years 20年后的人月神话

### 为什么会出现二十周年纪念版本？

- ？软件开发科学没有正确地发展
- ？人月神话仅仅是顺便提及了软件，而主要针对团队中的成员如何创建事物

### 核心观点：概念完整性和结构师

- 概念完整性
  - 一个整洁、优雅的编程产品必须向它的每个用户提供一个条理分明的概念模型，这个模型描述了应用、实现应用的方法以及用来指明操作和各种参数的用户界面使用策略
  - 必要的管理活动
- 结构师
  - 结构师是这些模型的所有者，同时也是用户的代理
- 将体系结构和设计实现、物理实现相分离
- 体系结构的递归
- 概念完整性是产品质量的核心，拥有一位结构师是迈向概念完整性的最重要一步

### 开发第二个系统所引起的后果：盲目的功能和频率猜测

- 为大型用户群设计
- 盲目的功能(Featuritis)
  - 以性能甚至是可用性为代价，过多地向 产品添加边界实用功能
- 定义用户群
- 频率
  - 结构师应该猜测或者假设完整的一系列属性和频率值
  - 清晰和错误都比模糊不清好得多

### 图形(WIMP)界面的成功

- 通过类比获得的概念完整性
  - 桌面的比喻
  - 菜单和单手操作
- 命令表达和双光标问题
- 用户功能和易用性的兼具
- 快捷键：新手到熟练用户的逐渐过渡
- 强制体系结构的实施，作为设备的直接整合
- 过时被淘汰

### 没有构建舍弃原型——瀑布模型是错误的

- 瀑布模型的谬误
  - 假设项目只经历一次过程，而且体系结构出色并易于使用，设计是合理可靠的，随着测试的进行，编码实现是可以修改和调整的
  - 假设整个系统一次性地被构建，在所有的设计、大部分编码、部分单元测试完成之后，才为闭环的系统测试合并各个部分
- 必须存在逆向移动

### 增量开发模型更佳——渐进地精化

- 构建闭环的框架系统
  - 可以很早开始用户测试
  - 可以采用按预算开发的策略
- Parnas产品族
  - 将软件作为一系列相关的产品族来设计
  - 将变化可能性较小的设计决策放置在树的根部
  - 模块重用的最大化
- Microsoft的“每晚重建”方法
- 增量式开发和快速原型

### 关于信息隐藏，Parnas是正确的，我是错误的

- 信息隐藏——现在常常内建于面向对象的编程中——是唯一提高软件设计水平的途径
- 把Parnas模块提升到抽象数据类型，从中可以派生出很多对象
  - 抽象数据类型提供了一种思考和指明模块接口的统一方式，以及容易保证实施的类型规范化访问方法
- 继承

### 人月到底有多少神话色彩？Boehm的模型和数据

- 向进度落后的软件项目中添加人手只会使进度更加落后

### 人就是一切（或者说，几乎是一切）

- 项目人员的素质、人员的组织管理是比使用的工具或采用的技术方法更重要的因素
- 人件
- 项目转移？团队的重要性

### 放弃权力的力量

- 通过权力委派，中心的权威实际上是得到了加强；从整体而言，组织机构实际上更加融洽和繁荣

### 最令人惊讶的新事物是什么？数百万的计算机

- 微型计算机革命改变了每个人使用计算机的方式
- 微型计算机革命改变了每个人开发软件的方式

### 全新的软件产业——塑料薄膜包装的成品软件

- 传统软件产业
  - 计算机提供商
  - 应用程序用户
  - 定制程序开发者
  - 商业包开发者
- 操作系统世界的统一
- 塑料薄膜包装的成品软件产业

### 买来开发——使用塑料包装的成品软件包作为构件

- 使用大众市场的软件包作为平台，在上面开发更丰富和更专业的产品
- 元编程：为部分软件包用户进行功能定制的过程
- 成品软件包提供了大型的功能模块和精心定制的接口，它内部的概念结构根本无需再设计
- 需要什么？
  - 直接使用用户
  - 元程序员，在单个应用程序的基础上，使用已提供的接口来开发模板或者函数
  - 外部工鞥作者，向应用程序中添加自行编制的功能
  - 元程序员，使用一个或者多个特殊的应用程序，作为更大型系统的构件

### 软件工程的状态和未来

- 软件工程的焦油坑在将来很长一段时间内会继续使人们举步维艰，无法自拔


## Epilogue Fifty Years of Wonder, Excitement, and Joy 结束语：令人向往、激动人心和充满乐趣的五十年

- 这个神奇的时代远远没有结束，它仍然在飞速发展。更多的乐趣，尽在将来