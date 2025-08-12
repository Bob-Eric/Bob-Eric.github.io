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

+ **编程：**熟练掌握Python、C++和C#，有嵌入式开发经验。
+ **机器人：**熟悉ROS，掌握主流定位与导航算法，具备丰富的机器人开发经验。
+ **AI与工具链：**能用PyTorch设计深度学习模型，熟练使用SolidWorks、Unity等工具

## 自我评价

+ **基础素质：**本硕均就读于天津大学，成绩优异，具备多学科交叉背景，自主学习能力强。
+ **项目经验：**参与多个跨学科项目，熟练多种编程语言及嵌入式和机械设计，具备良好团队协作能力。
+ **学习态度：**对机器人行业充满热情，关注前沿技术，积极学习新知，致力于将所学应用于实际。

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
  针对端到端越野规划器依赖高保真仿真或难以收集的真实数据，开发高性能仿真器及sim-to-real端到端规划器，仅用仿真数据训练，可直接部署于真实环境。
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
  提出一套自主机器人系统，实现长时序操作任务的sim-to-real迁移，感知与伺服模块针对运动模糊和抓取误差设计，仿真与现实均达亚厘米级精度。

  </div>
</div>

# 🏆 竞赛获奖 {#Awards}

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <img src='images/RMUS_snapshot.jpg' alt="RMUS snapshot" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

  **RoboMaster University Sim2Real Challenge (RMUS)&emsp;第一名&emsp;2023.12-2024.5**  

  作为队长，带领团队完成EP机器人自主搜寻与堆放矿石任务，核心为亚厘米精度视觉伺服，攻克运动模糊和控制解耦难题。

  **主要贡献：**  

  + **导航系统：**鉴于2D激光雷达+全向底盘配置，使用Cartographer定位，Teb导航。
  + **感知系统：**结合ArUco与LeNet分类器，实现1ms推理，0.6cm/1.9°精度。
  + **伺服系统：**反馈线性化解耦控制，系统辨识参数，实际达亚厘米精度。

  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <img src='images/RMUC_snapshot.jpg' alt="RMUS certificate" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

  **RoboMaster 2023赛季&emsp;联盟赛一等奖&emsp;超级对抗赛全国赛三等奖&emsp;2022.9-2023.9**

  负责哨兵机器人导航与决策功能。  

  **主要贡献：**

  + **方案设计：**采用2D激光雷达+工控机硬件，使用Cartographer SLAM，A*全局+Teb局部规划。
  + **串口通信：**使用明文字符串传输控制与心跳指令，主控超时接管。
  + **算法调试：**使用Gazebo仿真，运用状态机控制巡逻与扫描。

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

  **工作描述：**基于Unity开发无人机集群高保真仿真系统，验证通信、编队、任务分配、避碰、轨迹规划等能力。

  **主要贡献：**

  + **场景构建：**搭建机场与港口三维场景，构建29种任务目标模型，运用泊松盘采样在场景中动态生成目标。

  + **通信网络：**将Unity接入ROS，形成224架仿真和32架半实物无人机通信网络。

  + **性能评估：**使用层次分析法计算场景整体任务执行效果。

  + **用户界面：**使用Unity UI组件实现视角与场景管理、地图沙盘推演和性能评估结果可视化等其他设置。

  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <img src='images/Multi_agent_capture.jpg' alt="RMUS certificate" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

  **多智能体博弈动态覆盖策略研究&emsp;南开大学项目&emsp;2023.9-2023.12**

  **工作描述：**研究多智能体协同运动策略，计算覆盖所需数量，近距离采用动态攻防博弈决策。

  **主要贡献：**

  + **覆盖数量计算：**通过几何分析，推导围捕所需智能体数量的计算方法。
  + **动态攻防决策：**利用模糊决策树，根据对局态势动态选择机动与火力动作。

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

  **YOPO-Sim**&emsp;
  <img src="https://img.shields.io/github/stars/TJU-Aerial-Robotics/YOPO-Sim?style=social" alt="GitHub stars">&emsp;
  [[code](https://github.com/TJU-Aerial-Robotics/YOPO-Sim)]&emsp;
  所有者

  基于Unity开发的高性能、支持多传感器、兼容ROS的车辆越野仿真器。
    
  **主要功能：**

  + **多传感器支持：**集成多种传感器，包括RGB相机、深度相机、鱼眼相机、激光雷达和惯性测量单元。
  + **随机生成环境：**程序化批量生成多样化的越野地形和植被。
  + **数据生成：**批量保存多种数据，包括图像、车辆姿态和点云地图。
  + **ROS集成：**通过ROS TCP Connector与ROS无缝连接，实现实时数据流传输。
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

  **VoxelGenerator**&emsp;
  <img src="https://img.shields.io/github/stars/TJU-Aerial-Robotics/VoxelGenerator?style=social" alt="GitHub stars">&emsp;
  [[code](https://github.com/TJU-Aerial-Robotics/VoxelGenerator)]&emsp;
  所有者

  用于实时点云生成的Unity包，基于碰撞体生成体素点云。

  **主要功能：**

  + **实时生成：**实时生成大规模场景的点云数据。
  + **高性能：**采用分层并行检测策略，实现高效的体素生成。
  + **数据导出：**支持将点云数据导出为.ply和.pcd格式文件。
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

  **UnitySensors**&emsp;
  <img src="https://img.shields.io/github/stars/Field-Robotics-Japan/UnitySensors?style=social" alt="GitHub stars">&emsp;
  [[code](https://github.com/Field-Robotics-Japan/UnitySensors)]&emsp;
  贡献者

  基于Unity开发的高性能、兼容ROS的多种传感器模拟包。

  **主要贡献：**

  + 完善深度相机，以支持不同渲染管线
  + 增加坐标变换（TF）传感器
  + 增加鱼眼相机传感器，编写Shader采样立方体贴图，从像素坐标反求世界坐标，支持等距模型与EUCM模型
  </div>
</div>
