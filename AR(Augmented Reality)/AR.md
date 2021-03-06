# AR(Augmented Reality)

## Intro

- 一种将虚拟信息与真实世界巧妙融合的技术
- 关键技术
  - 跟踪注册技术
    - 虚拟信息和真实环境在三维环境的配准注册
    - 空间定位跟踪
    - 真实空间中的定位
  - 显示技术
  - 虚拟生物生成技术
  - 交互技术
    - 现实世界中的点位选取来进行交互
    - 姿势/手势交互
    - 特制工具交互
  - 合并技术
    - 将虚拟信息与输入的现实场景无缝结合
    - 几何一致、模型真实、光照一致、色调一致

- SLAM(simultaneous localiztion and mapping)/CML(Concurrent Mapping Localization) 即时定位与地图构建/并发建图与定位

## Animation Based Solutions

- QQ-AR
  - 上传识别图，以及展示视频，创建 AR 任务
  - AR 形象固定在手机摄像头画面，而不是基于场景的交互
  - 人脸识别，物体识别，姿势识别，3D 动画......
- 网易易现
  - 两款产品：网易洞见，网易影见
  - 网易洞见
    - 移动客户端的应用，依托SaaS云平台
    - 互联网应用引擎 AR SDK：问题在于商业合作，八成不开源
    - AR游戏引擎，同上
  - 网易影见
    - AR互动投影
    - 平面点击，空中手势，实物互动，图像识别
- 我的天科技
  - AR创意营销（基于各AR平台的营销服务）
  - AR应用服务
  - 企业AR云服务
  - AR-SDK嵌入服务
- 支付宝AR
  - 基于用户需求制作的营销服务
- 视+AR（基于EasyAR的解决方案提供商，与EasyAR同属上海视辰科技）
  - 各种AR解决方案
  - 移动应用AR集成方案
    - 提供基于EasyAR的一站式解决方案
    - 提供平台或者对接已有平台
    - 提供AR创意、AR内容制作
  - AR定制化解决方案
    - AR创意策划
    - AR内容定制
    - APP定制
    - 大屏AR互动方案定制
  - AR流量平台投放方案
  - WebAR解决方案（完全基于EasyAR）
  - AR绘本阅读解决方案（根据绘本图片播放音视频）
  - AR眼镜，AR大屏，AR远程协助，SLAM，AR云，微信、支付宝AR，AR导航
- AliGenie
  - 流程：申请开发包 -> 下载SDK -> 集成到自有APP -> 上传AR内容 -> 应用上线
  - SDK：云识别、NFT、微端次世代渲染、3D追踪和识别
    - 提供快速精准的识别、稳定的三维感知与跟踪和超轻量引擎渲染
    - ios 、Android
- ...

- 共同的特征：基于视频或者3d动画，无开发、编码要求


## Code Based Frameworks

- ARCore（比较硬核）
  - Google 提供的SDK
  - 多平台以及多建模引擎的SDK支持：ios/android, unity/unreal
  - 支持导入资产
  - 难度较大，文档不够详细
  - 待麒麟哥补充？

- ARKit
  - 仅限ios平台开发和使用，不考虑

- Vuforia
  - 待余佳怡补充？

- EasyAR
  - 介于解决方案和框架之间，可以借助平台提供的解决方案，也可以自由开发
  - 多种产品：
    - WebAR: 与解决方案类似，以二维码H5或者小程序展现
    - **EasyAR Sense SDK** （主要在于这个的开发）
      - SpatialMap的调用收费
    - EasyAR CRS 云端识别服务：基于云端的图像识别和检索服务（可以像解决方案一样，根据图像扫描识别后找到对应的3D模型）
    - EasyAR AI：基于AI，姿势、手势识别，除了少量标准库，可以借助平台训练（// 和洗手还是不太一样...洗手想做好的话还是要做机器学习）

- DuMix AR（百度AR）
  1. 虚拟形象生成驱动
  2. 人像美化
  3. 互动玩法
  4. 空间定位与显示增强
  5. 虚实融合渲染

- 共同特征：基于编码，基于空间地图，有交互，不是仅仅放视频那么简单，可以对交互做出反应。
