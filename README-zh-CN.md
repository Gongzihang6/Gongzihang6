<p align="right">
  <a href="./README.md"> English </a> | <b> 简体中文 </b>
</p>
<div align="center">
  <img src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif" width="100" />
  <h1> 你好，我是 <a href="https://gongzihang6.github.io/"> GZH </a>! <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30px"/> </h1>

  <h3> 👨‍🎓 数学硕士 (M.Sc.) | 🔭 SLAM & 3D 计算机视觉算法工程师 </h3>

  <p>
    <b> 💻 C++ 底层开发 | 🤖 多传感器融合 | 🏸 羽毛球运动员 </b>
  </p>

  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=2196F3&center=true&vCenter=true&width=500&lines=Coding+with+Math+and+C%2B%2B.;Building+SLAM+Systems.;Researching+3D+Point+Clouds.;Smashing+shuttles+on+court." alt="Typing SVG" />
  </a>
</div>

---

### 🌱 关于我 (About Me)

一名具备扎实数学功底（几何、优化、概率）的 **SLAM 与 3D 视觉算法工程师**。致力于将前沿的理论基础转化为高可靠的工程实现，深耕自动驾驶与机器人领域的空间感知技术。

* 🔭 **研究与实践**：多模态端到端自动驾驶大模型 (DLWM/BEV)、多传感器紧/半紧耦合 SLAM、3D 点云深度学习与大场景重建。
* 🎯 **核心优势**：从底层 C++ 系统架构（多线程/硬件同步）、到中间层核心算法推导（IESKF/因子图）、再到上层深度学习大模型（PTv3/3D Gaussian）的完整技术栈打通能力。
* 🏸 **个人爱好**：羽毛球狂热者，古诗词爱好者（“观史知今，当思进退”）。

---

### 🛠️ 技术栈与核心能力 (Tech Stack & Core Competencies)

<div align="center">

| **领域**        | **技术栈**                                                   |
| :-------------- | :----------------------------------------------------------- |
| **编程语言**    | ![C++](https://img.shields.io/badge/Modern_C++_11/14/17-00599C?style=flat-square&logo=c%2B%2B&logoColor=white) ![Python](https://img.shields.io/badge/Python_(uv)-3776AB?style = flat-square&logo = python&logoColor = white) ![Matlab](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white) |
| **SLAM & 视觉** | ![ROS2](https://img.shields.io/badge/ROS2-22314E?style=flat-square&logo=ros&logoColor=white) ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white) ![PCL](https://img.shields.io/badge/PCL-Point_Cloud_Library-blue?style=flat-square) ![Eigen](https://img.shields.io/badge/Eigen-Linear_Algebra-red?style=flat-square) |
| **优化理论**    | ![Ceres](https://img.shields.io/badge/Ceres_Solver-Optimization-green?style=flat-square) ![g2o](https://img.shields.io/badge/g2o-Graph_Optimization-orange?style=flat-square) ![GTSAM](https://img.shields.io/badge/GTSAM-Factor_Graphs-yellow?style=flat-square) |
| **AI 工具链**   | ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![Linux](https://img.shields.io/badge/Linux/WSL-FCC624?style=flat-square&logo=linux&logoColor=black) ![CMake](https://img.shields.io/badge/CMake-064F8C?style=flat-square&logo=cmake&logoColor=white) |

</div>

* ⚙️ **算法工程化与高性能计算**：精通 Modern C++，熟练掌握面向对象设计。擅长在 Linux/WSL 下使用 CMake 进行跨平台构建，具备深厚的内存管理、多线程并发处理及无锁队列实战经验。
* 🧭 **状态估计与多传感器融合**：精通李群与李代数，深刻理解 VIO/LIO 运行机制。掌握各类传感器的时空同步与联合标定方法，能熟练运用滤波（KF/IESKF）与图优化（Ceres/GTSAM）解决复杂的非线性状态估计问题。
* 👁️ **三维感知与自动驾驶前沿**：具备海量实车与异构传感器数据的处理经验。熟悉 3D 点云的底层几何处理（配准、滤波），并掌握主流 3D 深度学习大模型（PTv3, Swin3D, OctFormer, BEV, 3D Gaussian Splatting）在自动驾驶感知系统中的工程落地。

---

### 💼 工业界实战经历 (Industry Experience)

**岚图汽车 (Voyah) | 自动驾驶算法研发实习生** 

**项目一：基于 DLWM 的端到端自动驾驶 3D Gaussian 预训练**

-   **核心架构与特征解码：** 构建端到端自动驾驶 3D Gaussian 感知大模型。以 ResNet 配合 FPN 提取多视角图像多尺度特征，设计 Gaussian Transformer 解码器。利用 3D 稀疏卷积处理高斯基元间的自交互（Self-encoding），并通过可变形交叉注意力（Deformable Cross-attention）聚合 2D 图像特征，迭代回归高斯球的 3D 坐标、协方差与语义 logits。
-   **多模态联合自监督渲染闭环：** 构建基于 Alpha-blending 机制的高保真可微渲染监督流程。引入视觉基础大模型 SAM3 自动生成 2D 语义伪标签，并融合稀疏 LiDAR 点云与 Metric3D 稠密伪深度。在无需 3D 密集标注的条件下，通过 2D 视角的交叉熵与 L1 重建损失进行梯度回传，迫使 3D 高斯基元学习真实的 3D 物理几何与语义分布。
-   **落地成果：** 成功导出具备高鲁棒性的 3D 高斯场景表征，深度图预测平均绝对误差低至 **0.69m**，语义分割 mIoU 达到 **85.63%**，为下游 BEV 光栅化（Rasterization）与时空运动预测、轨迹规划提供了极强的场景理解先验。

**项目二：基于 BEVFusion 架构的多模态端到端规控网络**

-   **多传感器 BEV 统一与高斯解码：** 打通图像与点云的特征级融合链路。针对相机分支采用视锥深度估计完成 Camera-to-BEV 的精确投影，与 LiDAR BEV 特征在统一空间拼接后，利用全卷积 BEV 编码器消除局部不对齐，获取 `bev_fusion_feat`。随后接入定制的特征解码头，高效回归并导出 3D 高斯球参数。
-   **基于视觉大模型的高维语义蒸馏：** 引入预训练大模型 DINOv3 作为 Teacher 网络。将 3D 高斯特征通过光栅化渲染至多视角 2D 平面，构建与 DINOv3 提取特征的对比学习损失（Contrastive Loss）。通过图像、特征与 LiDAR 深度图的多重监督，引导底层 BEV 空间学习极具泛化性的开放世界语义表达。
-   **端到端无感知规控闭环：** 重构传统“感知-预测-规控”的级联架构。直接从富含 DINOv3 先验的 BEVFusion 特征中提取场景查询（Scene Queries），并与自车航点查询（Waypoint Queries）进行交互，回归规划轨迹。彻底摒弃车道线、OCC 等显式中间件，旨在大幅削减级联误差累积并缩短系统端到端延迟。

---

### 🚀 开源项目与核心研发 (Projects)

#### 1. C/S 架构多相机 3D 感知与大模型测量系统 (独立研发) 

面向复杂高噪环境的端到端软硬件 3D 感知流水线，打通从底层数据获取到三维几何特征提取的完整链路：

*   **多机高频采集与在线概率配准：** 基于 C++17 与 Qt，实现 5 台 **Orbbec Femto Bolt**（2.3m 架设高度）的硬件级微秒同步与数据采集系统。运用无锁队列构建异步 I/O 架构，保障多模态数据零延迟落盘。设计“离线外参粗对齐 + 在线 **G-ICP** 概率精配准”架构，基于马哈拉诺比斯距离度量（Mahalanobis Distance）有效克服活体非刚性曲面带来的配准发散。 
*   **类别不平衡优化与 3D 语义分割：** 实现 **OctFormer**、**Point Transformer v3 (PTv3)** 与 **Swin3D**。针对复杂养殖环境 1:6 的空间类别不平衡，创新引入 Focal Loss + Lovász-Softmax Loss，将模型注意力的梯度流精准锚定在粘连边界，精准剥离主体点云，测试集上实现 **Mean IoU/Recall/Precision 0.9839/0.9949/0.9955**。 
*   **多点共识关键点回归：** 设计 Bottom-up 的局部密集预测与空间投票机制，直接在 3D 空间中联合回归 P1 至 P6 六大生物解剖学关键点，定位平均误差低至 **21.62mm**。 
*   **几何拓扑测算与 SVR 归因预测：** 提出 PCA 姿态标准化与 **Catmull-Rom 闭合样条插值算法**，通过等角积分重构缺失的流形拓扑，消除活体低头、弯曲干扰。实测胸围、体高、体长相对误差 (MAPE) 均 $\le$ **4.63%**；将 3D 几何特征输入支持向量回归 (SVR) 模型，最终在独立测试集上达成 MAPE **3.88%**（57.5% 样本绝对误差 $\le$ **3kg**）的极高预测精度。

#### 2. 多传感器融合增强系统：FAST-LIVO2 深度改进
面向复杂环境下的长航时高精度定位需求，对主流 LIVO 框架进行底层改造与多源异构数据融合：
* **半紧耦合架构 (基于 GTSAM)：** 以 FAST-LIVO2 原系统输出位姿为局部先验，在 GTSAM 中构建关键帧位姿图，增加 **DBoW3 + TEASER++ + GICP refine** 的回环检测因子，同时将 GNSS 绝对位置约束、 Wheel 平面运动先验与回环因子统一纳入 iSAM2 增量优化框架，实现前端局部精度与后端全局一致性的解耦融合。在 `M3DGR Varying-illu05` 数据集上完成多组对比实验，后端融合后 ATE Mean 稳定由 **0.21~0.22 m 降至 0.067~0.070 m** ， ATE RMSE 由 **0.23~0.24 m 降至 0.076~0.079 m** ，相对下降约 **65%~70%**。
* **完全紧耦合探索 (基于 IESKF)：** 深入研究框架底层状态机制，独立推导 GNSS 与 Wheel 测量模型对误差状态变量的雅可比矩阵，将其直接作为观测残差项无缝融入原系统的 IESKF（迭代误差状态卡尔曼滤波）中，对比分析松耦合因子图与紧耦合滤波的建模边界、工程复杂度与鲁棒性差异，探索紧耦合理论边界。

#### 3. 动态场景鲁棒建图流水线：Semantic-FAST-LIO2
面向自动驾驶高精度真值 (Ground Truth) 生成需求，构建基于语义先验的高鲁棒离线建图数据闭环：
* **3D 分割模型部署：** 基于 `SemanticKITTI` 数据集训练部署 **Point Transformer v3 (PTv3)** 大模型，实现对点云级的高精度语义感知。
* **C++ 底层重构与融合：** 在 C++ 端利用 PCL 编写高效数据预处理模块，前置滤除高动态物体（人、车）的点云。将清洗后的纯静态环境结构与高频 IMU 数据实现严格的时间戳对齐，随后输入 FAST-LIO2 引擎进行位姿解算。
* **效果量化：** 熟练使用 `evo` 工具链进行轨迹对比分析。该方案从根本上消除了动态遮挡导致的“里程计退化”与“地图鬼影”问题。

#### 4. 农业动态场景目标检测与追踪 (CV & 启发式优化)
* **检测与跟踪架构：** 构建基于 YOLOv5/8 与 MOT（ByteTrack / Bot-SORT）结合的高精度流水线，解决密集遮挡与特征漂移痛点。
* **启发式全局寻优：** 针对深度学习超参数搜索空间大的问题，创新引入**遗传算法 (GA)、粒子群算法 (PSO) 及模拟退火算法 (SA)** 等数学智能优化策略，对学习率及 Anchor 尺寸等进行自动化寻优，使复杂验证集上的检测精度 **(mAP@50) 从 90.9% 提高到 95.04%**。

#### 5. 基于树模型集成与 SHAP 归因的房价预测 (数据挖掘)
* 利用 VIF 检验共线性，结合 KDE 分析底层分布进行深度特征工程。搭建并深挖 GBDT、XGBoost、LightGBM 的二阶泰勒展开优化策略，最终 XGBoost 取得 $R^2$ **0.845**、MAPE **16.2%** 的最优性能。
* 引入 **SHAP** 值打破黑盒效应，生成特征力图与决策图，直观量化特征正负向贡献，打通模型的业务解释闭环。


---

### 🗺️ 学习路线与里程碑 (Roadmap)

#### 📚 理论基础 & 书籍
- [x] **视觉 SLAM 十四讲** - *打下坚实数学与推导基础*
- [x] **自动驾驶与机器人中的 SLAM 技术** - *理论走向工程实践的桥梁*
- [ ] **机器人学中的状态估计** (Barfoot) - *深耕估计理论与非线性优化数学原理*

#### 🔭 SLAM 系统 & 源码重构
- [x] **FAST-LIO2 / FAST-LIVO2** - *深入理解 IESKF 以及紧耦合 LIO/VIO 架构*
- [x] **VINS-Mono** - *研究滑动窗口优化、预积分与边缘化机制*
- [x] **ORB-SLAM2** - *稀疏特征点法与多线程系统工程解析*

#### 🧠 3D 深度学习大模型
- [x] **Point Transformer 系列 (V1/V2/V3)** - *点云注意力机制与语义分割实践*
- [x] **Swin3D / OctFormer** - *分层 Transformer 架构及八叉树高效表征*
- [x] **3D Gaussian Splatting / DLWM / BEVFusion** - *端到端场景重建与多模态表征前沿*

---

### 🏆 荣誉奖项 (Honors)

* **国家级：** 华为杯中国研究生数学建模竞赛 **国家二等奖** | 正大杯全国大学生市场调查与分析大赛 **国家三等奖** | MCM/ICM 美赛 **HM 奖**
* **校省级：** 全国大学生数学竞赛 **一等奖** | 英语口语 **一等奖**

---

### 📫 联系我 (Connect)

<div align="center">

<a href="https://x.com/ZihangGong28792_" target="_blank">
  <img src="https://img.shields.io/badge/X-%23000000.svg?style=for-the-badge&logo=X&logoColor=white" alt="X"/>
</a>

<a href="https://t.me/gongzihang" target="_blank">
  <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram"/>
</a>

<a href="mailto:zihanggong24@gmail.com" target="_blank">
  <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail"/>
</a>

<a href="https://space.bilibili.com/688234000" target="_blank">
  <img src="https://img.shields.io/badge/Bilibili-00A1D6?style=for-the-badge&logo=bilibili&logoColor=white" alt="Bilibili"/>
</a>

<a href="https://www.zhihu.com/people/qia-bu-qi-nuo-68-14" target="_blank">
  <img src="https://img.shields.io/badge/Zhihu-0084FF?style=for-the-badge&logo=zhihu&logoColor=white" alt="Zhihu"/>
</a>

<a href="https://blog.csdn.net/weixin_57248649" target="_blank">
  <img src="https://img.shields.io/badge/CSDN-FC5531?style=for-the-badge&logo=rss&logoColor=white" alt="CSDN"/>
</a>

<a href="https://www.cnblogs.com/gzhBlogs" target="_blank">
  <img src="https://img.shields.io/badge/CNBlogs-2ea44f?style=for-the-badge&logo=rss&logoColor=white" alt="CNBlogs"/>
</a>

</div>

<p align="center">
  <i> "数学是科学的皇后，而数论是数学的皇后。" </i>
</p>
