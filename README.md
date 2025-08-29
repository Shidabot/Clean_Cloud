# SLAM Project

本项目实现了一个基础的 **Simultaneous Localization and Mapping (SLAM)** 系统，包括前端特征提取、后端优化以及地图构建。
![SLAM Demo](./demo1.gif) ![SLAM Demo](./demo2.gif)
## 功能特性
- [x] 前端：特征提取与匹配（ORB/SIFT 可选）
- [x] 后端：位姿图优化（基于 g2o / Ceres）
- [x] 回环检测
- [x] 地图可视化

## 环境依赖
- Ubuntu 20.04 / 22.04
- ROS Noetic / ROS2 (可选)
- C++17
- Eigen3
- OpenCV >= 4.0
- Pangolin (可视化)
- g2o / Ceres

安装依赖示例：
```bash
sudo apt-get install libeigen3-dev libopencv-dev
