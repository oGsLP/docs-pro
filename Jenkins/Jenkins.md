# Jenkins

## 什么是 Jenkins

- Java 编写，开源的/提供友好人机交互界面的 CI&CD 工具，用于持续，自动的构建/测试软件项目，监控外部任务的运行，支持系统包/Docker/独立程序运行
- CI&CD
  - 持续集成，持续交付/部署，进行产品的快速迭代
  - 构成一个良好的 DevOps 环境，提升开发效率
- 通过流水线编排自动化构建过程

## Jenkins 的安装

0. 准备
   - 一定的内存与空间
   - Java 8 / Docker
1. 下载 <http://mirrors.jenkins.io/war-stable/latest/jenkins.war(https://mirrors.huaweicloud.com/jenkins/war/latest/jenkins.war>)
2. 下载目录下打开终端，运行`java -jar jenkins.war --httpPort=8080`
3. 浏览器打开 <http://localhost:8080> 按照说明安装

- 也可以通过 docker 运行 jenkins 的镜像

## Jenkins 的使用

1. 创建流水线
2. 配置流水线（项目 url，Jenkinsfile）
3. 流水线运行

## Jenkinsfile Pipeline

- 流水线 Pipeline，是用户定义的一个持续交付的流水线模型，定义了整个构建过程。将流水线定义到 Jenkinsfile 为最佳实践
  - 节点 node：机器，Jenkins 环境的一部分
  - 阶段 stage：整个流水线的执行任务中概念性不同子集
  - 步骤 step：一个单一的任务
- Jenkinsfile 常用语法
  - groovy 语法，可用声明式或脚本式格式，推荐**声明式**
  - 顶层 `pipeline{ ... }`
    1. Sections 节段
       - 一个节段通常包括一个或多个指令(Directives)或步骤(Steps)
       - agent 代理段
         - 指定整个流水线或特定的部分将会在 Jenkins 环境中执行的位置
         - 必须在 pipeline 顶层中定义，在 stage 中的定义是可选择的
         - any，none，label，node，docker，dockerfile...
       - stages 阶段段
         - 包含一系列 stage 指令
       - steps 步骤段
         - 在给定的 stage 中执行的定义一系列的步骤、
    2. Directives 指令
       - environment 环境
         - 键值对，根据指令在流水线中所处的位置定义了环境变量
       - options 选项
         - 在流水线内部配置特定于流水线的选项
         - timeout。etry，timestamps....
       - params 参数
         - 设置当前作用域下的可用参数值，有 string 和 boolean 类型
       - triggers 触发器
         - 定义了流水线被重新触发的自动化方法
         - cron，pollSCM，upstream
       - stage 阶段
         - 封装在 stages 中的一系列工作
       - tools 工具
         - 自动安装和放置 PATH 的工具的一部分
         - maven，jdk，gradle
       - input 输入
         - 定义提示输入，需要批准
       - when 条件判断
         - 允许流水线根据给定的条件决定是否执行该阶段
         - branch，environment，expression，not，allOf，anyOf
         - 在进入 stage 的 agent 前评估 when
    3. Parallel 并行
       - 在流水线的阶段中声明多个嵌套阶段并行执行
       - 包含 parallel 的 stage 不能包含 agent 和 tools，因为阶段中没有相关的 steps
    4. Steps 步骤
       - 一般的步骤如 bat/sh 等
       - script 脚本
         - 可以编写脚本加强流水线的功能
