<p align="right">
  <b> English </b> | <a href="./README-zh-CN.md"> 简体中文 </a>
</p>
<div align="center">
  <img src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif" width="100" />
  <h1> Hi, I'm <a href="https://gongzihang6.github.io/"> GZH </a>! <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30px"/> </h1>

  <h3> 👨‍🎓 M.Sc. in Mathematics | 🔭 SLAM & 3D Computer Vision Algorithm Engineer </h3>

  <p>
    <b> 💻 Low-level C++ Development | 🤖 Multi-Sensor Fusion | 🏸 Badminton Player </b>
  </p>

  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=2196F3&center=true&vCenter=true&width=500&lines=Coding+with+Math+and+C%2B%2B.;Building+SLAM+Systems.;Researching+3D+Point+Clouds.;Smashing+shuttles+on+court." alt="Typing SVG" />
  </a>
</div>

---

### 🌱 About Me

A **SLAM and 3D Vision Algorithm Engineer** with a solid mathematical foundation (Geometry, Optimization, Probability). I am dedicated to translating cutting-edge theoretical foundations into highly reliable engineering implementations, deeply engaged in spatial perception technologies for autonomous driving and robotics.

* 🔭 **Research & Practice**: Multi-modal end-to-end autonomous driving foundation models (DLWM/BEV), tightly/semi-tightly coupled multi-sensor SLAM, 3D point cloud deep learning, and large-scale scene reconstruction.
* 🎯 **Core Competency**: Ability to bridge the full technical stack, from low-level C++ system architecture (multi-threading/hardware synchronization), through middle-layer core algorithm derivation (IESKF/Factor Graphs), to upper-layer deep learning foundation models (PTv3/3D Gaussian).
* 🏸 **Hobbies**: Badminton enthusiast, lover of classical literature and poetry ("Observing history to understand the present; knowing when to advance and when to retreat").

---

### 🛠️ Tech Stack & Core Competencies

<div align="center">

| **Domain**        | **Tech Stack**                                               |
| :---------------- | :----------------------------------------------------------- |
| **Programming**   | ![C++](https://img.shields.io/badge/Modern_C++_11/14/17-00599C?style=flat-square&logo=c%2B%2B&logoColor=white) ![Python](https://img.shields.io/badge/Python_(uv)-3776AB?style=flat-square&logo=python&logoColor=white) ![Matlab](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white) |
| **SLAM & Vision** | ![ROS2](https://img.shields.io/badge/ROS2-22314E?style=flat-square&logo=ros&logoColor=white) ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white) ![PCL](https://img.shields.io/badge/PCL-Point_Cloud_Library-blue?style=flat-square) ![Eigen](https://img.shields.io/badge/Eigen-Linear_Algebra-red?style=flat-square) |
| **Optimization**  | ![Ceres](https://img.shields.io/badge/Ceres_Solver-Optimization-green?style=flat-square) ![g2o](https://img.shields.io/badge/g2o-Graph_Optimization-orange?style=flat-square) ![GTSAM](https://img.shields.io/badge/GTSAM-Factor_Graphs-yellow?style=flat-square) |
| **AI Toolchain**  | ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![Linux](https://img.shields.io/badge/Linux/WSL-FCC624?style=flat-square&logo=linux&logoColor=black) ![CMake](https://img.shields.io/badge/CMake-064F8C?style=flat-square&logo=cmake&logoColor=white) |

</div>

* ⚙️ **Algorithm Engineering & High-Performance Computing**: Proficient in Modern C++, mastering Object-Oriented Design. Adept at cross-platform builds using CMake in Linux/WSL, with extensive practical experience in memory management, multi-threading concurrency, and lock-free queues.
* 🧭 **State Estimation & Multi-Sensor Fusion**: Proficient in Lie Groups and Lie Algebras, with a deep understanding of VIO/LIO mechanisms. Master of spatio-temporal synchronization and joint calibration methods for various sensors. Skilled in applying filtering (KF/IESKF) and graph optimization (Ceres/GTSAM) to solve complex non-linear state estimation problems.
* 👁️ **3D Perception & Autonomous Driving Frontiers**: Rich experience in processing massive real-world vehicle and heterogeneous sensor data. Familiar with low-level geometric processing of 3D point clouds (registration, filtering), and proficient in the engineering deployment of mainstream 3D deep learning foundation models (PTv3, Swin3D, OctFormer, BEV, 3D Gaussian Splatting) in autonomous driving perception systems.

---

### 💼 Industry Experience

**Voyah | Autonomous Driving Algorithm R&D Intern** **Project 1: End-to-End Autonomous Driving 3D Gaussian Pre-training based on DLWM**
- **Core Architecture & Feature Decoding:** Built an end-to-end autonomous driving 3D Gaussian perception foundation model. Extracted multi-scale features from multi-view images using ResNet and FPN, and designed a Gaussian Transformer decoder. Processed self-encoding interactions between Gaussian primitives using 3D sparse convolutions, and aggregated 2D image features via Deformable Cross-attention to iteratively regress the 3D coordinates, covariance, and semantic logits of Gaussian spheres.
- **Multi-Modal Joint Self-Supervised Rendering Loop:** Constructed a high-fidelity differentiable rendering supervision pipeline based on the Alpha-blending mechanism. Introduced the vision foundation model SAM3 to automatically generate 2D semantic pseudo-labels, fused with sparse LiDAR point clouds and Metric3D dense pseudo-depth. Without requiring 3D dense annotations, gradient backpropagation was performed via 2D-view cross-entropy and L1 reconstruction loss, forcing 3D Gaussian primitives to learn real 3D physical geometry and semantic distributions.
- **Deployment Results:** Successfully exported a highly robust 3D Gaussian scene representation. The Mean Absolute Error (MAE) for depth map prediction was reduced to **0.69m**, and the semantic segmentation mIoU reached **85.63%**, providing strong scene understanding priors for downstream BEV rasterization, spatio-temporal motion prediction, and trajectory planning.

**Project 2: Multi-Modal End-to-End Planning & Control Network based on BEVFusion**
- **Multi-Sensor BEV Unification & Gaussian Decoding:** Bridged the feature-level fusion pipeline of images and point clouds. For the camera branch, applied frustum depth estimation for accurate Camera-to-BEV projection; concatenated with LiDAR BEV features in a unified space, and utilized a fully convolutional BEV encoder to eliminate local misalignments, extracting `bev_fusion_feat`. Subsequently, connected a customized feature decoding head to efficiently regress and export 3D Gaussian sphere parameters.
- **High-Dimensional Semantic Distillation based on Vision Foundation Models:** Introduced the pre-trained foundation model DINOv3 as the Teacher network. Rendered 3D Gaussian features onto multi-view 2D planes via rasterization, and constructed a Contrastive Loss against features extracted by DINOv3. Through multiple supervisions from images, features, and LiDAR depth maps, guided the low-level BEV space to learn highly generalizable open-world semantic representations.
- **End-to-End Integrated Planning & Control Loop:** Restructured the traditional cascaded "perception-prediction-planning" architecture. Directly extracted Scene Queries from BEVFusion features (enriched with DINOv3 priors) and interacted them with ego-vehicle Waypoint Queries to regress planning trajectories. Completely discarded explicit middleware such as lane lines and OCC, aiming to significantly reduce cascaded error accumulation and shorten system end-to-end latency.

---

### 🚀 Projects & Open Source

#### 1. C/S Architecture Multi-Camera 3D Perception & Foundation Model Measurement System (Independent R&D)
An end-to-end software/hardware 3D perception pipeline aimed at complex, high-noise environments, bridging the entire process from low-level data acquisition to 3D geometric feature extraction:
* **Multi-Camera High-Frequency Acquisition & Online Probabilistic Registration:** Based on C++17 and Qt, achieved hardware-level microsecond synchronization and data acquisition for 5 **Orbbec Femto Bolt** depth cameras (mounted at 2.3m). Constructed an asynchronous I/O architecture using lock-free queues to ensure zero-latency saving of multi-modal data. Designed an "offline extrinsic coarse alignment + online **G-ICP** probabilistic fine registration" framework, effectively overcoming registration divergence caused by live non-rigid curved surfaces using Mahalanobis Distance metrics.
* **Class Imbalance Optimization & 3D Semantic Segmentation:** Deployed **OctFormer**, **Point Transformer v3 (PTv3)**, and **Swin3D**. To address the severe 1:6 spatial class imbalance in complex breeding environments, innovatively introduced Focal Loss + Lovász-Softmax Loss to precisely anchor the gradient flow of model attention to adhered boundaries, accurately stripping the main body point cloud. Achieved a **Mean IoU/Recall/Precision of 0.9839/0.9949/0.9955** on the test set.
* **Multi-Point Consensus Keypoint Regression:** Designed a bottom-up local dense prediction and spatial voting mechanism to jointly regress six major anatomical keypoints (P1 to P6) directly in 3D space, lowering the average localization error to **21.62mm**.
* **Geometric Topological Measurement & SVR Predictive Attribution:** Proposed a PCA posture standardization and **Catmull-Rom closed spline interpolation algorithm** to reconstruct missing manifold topologies via equiangular integration, eliminating interference from live subjects lowering heads or bending. Measured Chest Girth, Body Height, and Body Length with relative errors (MAPE) $\le$ **4.63%**. Inputting 3D geometric features into a Support Vector Regression (SVR) model ultimately achieved an extremely high prediction accuracy with a MAPE of **3.88%** (57.5% of samples with absolute error $\le$ **3kg**) on the independent test set.

#### 2. Multi-Sensor Fusion Enhancement System: Deep Improvement of FAST-LIVO2
Addressing the demand for long-duration, high-precision positioning in complex environments, profoundly modified the mainstream LIVO framework with multi-source heterogeneous data fusion:
* **Semi-Tightly Coupled Architecture (based on GTSAM):** Using the raw pose output of FAST-LIVO2 as a local prior, built a keyframe pose graph in GTSAM. Added loop closure detection factors via **DBoW3 + TEASER++ + GICP refine**, while uniformly integrating GNSS absolute position constraints, Wheel planar motion priors, and loop closure factors into the iSAM2 incremental optimization framework, achieving decoupled fusion of frontend local accuracy and backend global consistency. Conducted multiple comparative experiments on the `M3DGR Varying-illu05` dataset; after backend fusion, ATE Mean stably dropped from **0.21~0.22 m to 0.067~0.070 m**, and ATE RMSE dropped from **0.23~0.24 m to 0.076~0.079 m** (a relative decrease of approx. **65%~70%**).
* **Fully Tightly Coupled Exploration (based on IESKF):** Delved into the framework's low-level state mechanism, independently derived the Jacobian matrices of GNSS and Wheel measurement models concerning error state variables, and seamlessly integrated them as observation residual terms directly into the original system's IESKF (Iterated Error-State Kalman Filter). Comparatively analyzed the modeling boundaries, engineering complexity, and robustness differences between loosely coupled factor graphs and tightly coupled filtering to explore the theoretical boundaries of tight coupling.

#### 3. Robust Mapping Pipeline for Dynamic Scenes: Semantic-FAST-LIO2
Geared towards the demand for high-precision Ground Truth (GT) generation in autonomous driving, constructed a highly robust offline mapping data loop based on semantic priors:
* **3D Segmentation Model Deployment:** Trained and deployed the **Point Transformer v3 (PTv3)** foundation model based on the `SemanticKITTI` dataset to achieve high-precision semantic perception at the point-cloud level.
* **C++ Low-Level Refactoring & Fusion:** Wrote an efficient data preprocessing module in C++ using PCL to filter out point clouds of highly dynamic objects (pedestrians, vehicles) in advance. Strictly aligned the cleaned pure static environmental structures with high-frequency IMU data by timestamps, and then fed them into the FAST-LIO2 engine for pose calculation.
* **Effect Quantification:** Proficiently utilized the `evo` toolchain for trajectory comparative analysis. This approach fundamentally eliminated "odometry degradation" and "map ghosting" issues caused by dynamic occlusions.

#### 4. Object Detection & Tracking in Dynamic Agricultural Scenes (CV & Heuristic Optimization)
* **Detection & Tracking Architecture:** Built a high-precision pipeline combining YOLOv5/8 and MOT (ByteTrack / Bot-SORT) to solve pain points of dense occlusion and feature drift.
* **Heuristic Global Optimization:** Addressing the large hyperparameter search space in deep learning, innovatively introduced mathematical intelligent optimization strategies such as **Genetic Algorithm (GA), Particle Swarm Optimization (PSO), and Simulated Annealing (SA)** to automatically optimize learning rates, Anchor sizes, etc., boosting detection accuracy **(mAP@50) from 90.9% to 95.04%** on complex validation sets.

#### 5. House Price Prediction based on Tree Model Ensembles and SHAP Attribution (Data Mining)
* Conducted deep feature engineering by testing collinearity with VIF and analyzing underlying distributions using KDE. Built and deeply explored the second-order Taylor expansion optimization strategies of GBDT, XGBoost, and LightGBM. Ultimately, the XGBoost model achieved an optimal performance of $R^2$ **0.845** and MAPE **16.2%**.
* Introduced **SHAP** values to break the black-box effect, generating feature force plots and decision plots to intuitively quantify the positive and negative contributions of features, bridging the business interpretation loop of the model.

---

### 🗺️ Learning Roadmap & Milestones

#### 📚 Theoretical Foundations & Books
- [x] **14 Lectures on Visual SLAM** - *Laying a solid mathematical and theoretical foundation*
- [x] **SLAM Technologies in Autonomous Driving and Robotics** - *A bridge from theory to engineering practice*
- [ ] **State Estimation for Robotics (Barfoot)** - *Deepening knowledge of estimation theory and the mathematical principles of non-linear optimization*

#### 🔭 SLAM Systems & Source Code Analysis
- [x] **FAST-LIO2 / FAST-LIVO2** - *Deep understanding of IESKF and tightly-coupled LIO/VIO architectures*
- [x] **VINS-Mono** - *Studying sliding window optimization, pre-integration, and marginalization mechanisms*
- [x] **ORB-SLAM2** - *Analyzing sparse feature-based methods and multi-threading system engineering*

#### 🧠 3D Deep Learning Foundation Models
- [x] **Point Transformer Series (V1/V2/V3)** - *Point cloud attention mechanisms and semantic segmentation practices*
- [x] **Swin3D / OctFormer** - *Hierarchical Transformer architectures and efficient Octree representations*
- [x] **3D Gaussian Splatting / DLWM / BEVFusion** - *Frontiers in end-to-end scene reconstruction and multi-modal representation*

---

### 🏆 Honors & Awards

* **National Level:** **National 2nd Prize**, "Huawei Cup" China Post-Graduate Mathematical Contest in Modeling | **National 3rd Prize**, "Zhengda Cup" National College Student Market Research and Analysis Competition | **Honorable Mention (HM)**, MCM/ICM
* **Provincial/University Level:** **1st Prize**, Chinese Mathematics Competitions (CMC) | **1st Prize**, Spoken English Competition

---

### 📫 Connect with Me

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
  <i> "Mathematics is the queen of the sciences, and number theory is the queen of mathematics." </i>
</p>
