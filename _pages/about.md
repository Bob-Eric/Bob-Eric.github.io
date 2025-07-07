---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

# 🎓 教育背景 {#Education}

## 教育经历

|   学校   |           学院           |   专业   |     学位     |     时间      |
| :------: | :----------------------: | :----: | :----------: | :-----------: |
| 天津大学 | 电气自动化与信息工程学院 | 自动化 | 硕士（推免） | 2023.9-2026.6 |
| 天津大学 |       未来技术学院       | 自动化 |     本科     | 2019.9-2023.6 |

## 专业技能

+ **编程：**熟练掌握Python、C++和C\#，具备扎实的编程基础和丰富的实践经验，有STM32等嵌入式开发经验。
+ **机器人：**熟悉ROS生态，掌握主流定位与导航算法，具备丰富的机器人开发经验，可快速搭建仿真环境。
+ **深度学习：**熟悉PyTorch深度学习框架，具备深度学习算法开发经验，能够独立设计和优化深度学习模型。
+ **软件：**熟练使用SolidWorks、Vim、Docker与Unity引擎，可使用Valgrind等工具调试内存泄漏与多线程。

## 自我评价

+ **基础素质：**本硕均就读于天津大学，成绩优异。具备自动化、机械等多学科交叉的专业背景，为在机器人领域的深入研究奠定了坚实基础。自主学习能力较强，能够快速掌握新知识和技术。
+ **项目经验：**在多个跨学科项目中担任不同角色，积累了丰富的项目开发经验，熟练运用多种编程语言以及嵌入式和机械设计等技术。能够独立完成复杂项目的全流程开发，具备良好的团队协作和沟通能力。
+ **学习态度：**对机器人行业充满热情，始终关注前沿技术动态，积极学习新知识，不断提升自我。致力于将所学知识应用于实际项目中，以实现个人价值与行业发展的紧密结合。

# 📝 学术成果 {#Publications}

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">Arxiv</div>
      <img src='images/YOPO-Rally_paperbox.png' alt="YOPO-Rally overview" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

  **YOPO-Rally: A Sim-to-Real Single-Stage Planner for Off-Road Terrain**

  **Hongyu Cao**, Junjie Lu, Xuewei Zhang, Yulin Hui, Zhiyu Li, and Bailing Tian

  [[paper](https://arxiv.org/abs/2505.18714)] [[code](https://github.com/TJU-Aerial-Robotics/YOPO-Rally)]

  针对端到端车辆越野规划器依赖高保真仿真数据或难以收集的真实数据，开发一套高性能仿真器及零微调sim-to-real端到端规划器。仿真器用于生成高保真训练数据，规划器输入深度图及当前状态预测轨迹，仅使用仿真数据训练，可直接部署于真实树林环境。

  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">ICRA 2025</div>
      <img src='images/RMUS_paperbox.jpg' alt="RMUS overview" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

  **Robotic Sim-to-Real Transfer for Long-Horizon Pick-and-Place Tasks in the Robotic Sim2Real Competition**

  Ming Yang*, **Hongyu Cao\***, Lixuan Zhao, Chenrui Zhang, and Yaran Chen

  *Equal contribution

  [[paper](https://arxiv.org/abs/2503.11012)] [[code](https://github.com/Bob-Eric/rmus2024_solution_ZeroBug)]

  我们提出了一套自主机器人系统，可在长时序操作任务中实现仿真到现实（sim-to-real）的迁移。该系统的核心在于其感知与伺服模块，分别针对运动模糊和抓取模拟误差进行了鲁棒设计，从而在仿真和现实中一致地达到了亚厘米级的视觉伺服精度。

  </div>
</div>


# 🏆 竞赛获奖 {#Awards}

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <img src='images/RMUS_snapshot.jpg' alt="RMUS snapshot" width="100%">
      <img src='images/RMUS_cetificate.jpg' alt="RMUS certificate" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

  **RoboMaster University Sim2Real Challenge (RMUS)&emsp;第一名&emsp;2023.12-2024.5**

  **工作描述：**作为队长，带领团队完成RoboMaster EP机器人在场地中自主搜寻散落的矿石（编号1-6的边长5cm的立方体）并在指定区域处按指定顺序尽可能高地堆放的任务。核心功能是亚厘米精度视觉伺服，核心难点是运动模糊克服和控制解耦。

  **主要贡献：**

  + **导航系统：**鉴于2D激光雷达与全向底盘配置，利用Cartographer定位，使用Teb规划器导航。

  + **感知系统：**由于ArUco可准确快速定位标签，但其基于匹配的方式识别编号易受运动模糊影响，而LeNet图像分类器识别编号鲁棒性好。二者结合搭建感知模块，通过拒识机制抵抗运动模糊，实现**1ms**的CPU推理时间及**0.6cm/1.9°**的位姿估计精度（1m内）。

  + **伺服系统：**针对立方体矿石斜向抓取侧滑问题，通过反馈线性化将全向底盘位置和姿态解耦以同时控制；通过系统辨识确定纯滞后与死区等参数，据此进行控制器仿真与设计，最终在实际中达到**亚厘米级**的伺服精度，高质量完成对所有矿石的抓取和堆叠。

  **工作成果：**以第一作者身份发表ICRA会议论文1篇（已录用），并在ICRA 2024 RMUS比赛中荣获第一名。

  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <img src='images/RMUC_snapshot.jpg' alt="RMUS certificate" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

  **RoboMaster 2023赛季&emsp;联盟赛第一名&emsp;国赛二等奖&emsp;2022.9-2023.9**

  **工作描述：**自该赛季开始，哨兵机器人全自主化，需根据规则在场地中自主移动、攻击与防御。我负责哨兵机器人导航与决策功能的实现。

  **主要贡献：**

  + **方案设计：**（1）鉴于比赛场地较为扁平，同时兼顾硬件成本与计算能力，选用2D激光雷达和工控机。（2）采用Cartographer SLAM算法，其融合激光雷达、IMU与轮式里程计以提高精度。（3）使用ROS导航框架，配置A*作为全局规划器，配置Teb作为局部规划器。
  + **串口通信：**上位机使用串口与底盘主控通信，接收并解包IMU、里程计与裁判系统信息，为方便调试，以明文字符串发送速度控制信息，该控制信息同时充当心跳信号。主控未按时收到心跳信息时，将接管控制权。
  + **算法调试：**（1）考虑到Gazebo与ROS无缝兼容，使用Gazebo搭建仿真环境。（2）使用状态机控制机器人巡逻、扫描与停止。

  </div>
</div>

# 🛠️ 项目经历 {#Projects}

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <img src='images/Simulator_setup.jpg' alt="RMUS certificate" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

  **基于任务场景的通信集群联合仿真系统开发&emsp;XXX项目&emsp;2023.9-2024.9**

  **工作描述：**基于Unity开发一套用于无人机集群在机场和港口环境中执行任务的高保真硬件在环仿真系统，以对其核心能力进行综合验证，包括通信网络、编队保持、任务分配、避碰、轨迹规划和性能评估。

  **主要贡献：**

  + **场景构建：**搭建机场与港口三维场景，构建29种任务目标模型，运用泊松盘采样在场景中动态生成目标。

  + **通信网络：**通过ROS TCP Connector将Unity接入ROS，形成224架仿真和32架半实物无人机通信网络。

  + **性能评估：**借助层次分析法，通过判断矩阵计算目标个体权重，从而计算场景整体任务执行效果。

  + **用户界面：**使用Unity的UI组件实现视角与场景管理、地图沙盘推演和性能评估结果可视化等其他设置。

  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <img src='images/Multi_agent_capture.jpg' alt="RMUS certificate" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

  **多智能体博弈动态覆盖策略研究&emsp;南开大学项目&emsp;2023.8-2023.11**

  **工作描述：**以多智能体动态围捕问题为背景，研究在我方智能体性能参数弱于敌方，但数量多于敌方情景下的多智能体协同运动策略，以覆盖围捕博弈目标。给定双方智能体参数条件下，计算覆盖所需的我方智能体数量。其次，双方接近时，运用更加精细的动态攻防博弈决策。

  **主要贡献：**

  + **覆盖数量计算：**通过几何方法分析，我方打击范围与敌方逃逸范围构成以双方初始位置为圆心，我方总打击距离与敌方行驶距离为半径的两个圆形，两圆交点对应的圆心角即为我方智能体围捕覆盖角，其与行驶时间相关，求导获得最大覆盖角，进而得出覆盖所需的我方智能体数量。

  + **动态攻防决策：**双方接近时，通过模糊决策树进行动态攻防。根据6种对局态势构建输入特征指标集，根据4种机动动作与2种火力动作构建输出决策属性集，通过预定义的专家决策训练集，生成机动决策树与火力决策树。

  </div>
</div>

# 💻 开源项目 {#OpenSource}

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">Unity</div>
      <img src='images/YOPO-Sim.jpg' alt="YOPO-Sim" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

  **YOPO-Sim** [[code](https://github.com/TJU-Aerial-Robotics/YOPO-Sim)]&emsp;Owner

  基于Unity开发的高性能、支持多传感器、兼容ROS的车辆越野仿真器。
    
  + **多传感器支持：**集成多种传感器，包括RGB相机、深度相机、鱼眼相机、激光雷达（LiDAR）和惯性测量单元（IMU）。
  + **随机生成环境：**程序化批量生成多样化的越野地形和植被。
  + **数据生成：**批量保存多种数据，包括图像、车辆姿态和点云地图。
  + **ROS集成：**通过ROS TCP Connector与ROS无缝连接，实现实时数据流传输。
  + **高保真模拟：**为自动驾驶车辆越野研究提供逼真的模拟环境。
  </div>
</div>


<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">Unity</div>
      <img src='images/VoxelGenerator.jpg' alt="VoxelGenerator" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

  **VoxelGenerator** [[code](https://github.com/TJU-Aerial-Robotics/VoxelGenerator)]&emsp;Owner

  用于实时点云生成的Unity包，基于碰撞体生成体素点云。

  + **实时生成：**实时生成大规模场景的点云数据。
  + **高性能：**采用分层并行检测策略，实现高效的体素生成。
  + **数据导出：**支持将点云数据导出为.ply和.pcd格式文件。
  + **可扩展性：**采用干净且模块化的代码结构，便于定制和扩展。
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">Unity</div>
      <img src='images/UnitySensors.jpg' alt="UnitySensors" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

  **UnitySensors** [[code](https://github.com/Field-Robotics-Japan/UnitySensors)]&emsp;Contributor

  基于Unity开发的高性能、兼容ROS的多种传感器模拟包。

  **主要贡献：**
  + 完善深度相机，以支持不同渲染管线
  + 增加坐标变换（TF）传感器
  + 增加鱼眼相机传感器，编写Shader采样立方体贴图，从像素坐标反求世界坐标，支持等距模型与EUCM模型
  </div>
</div>