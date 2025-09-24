# Clean and Consistent MLS Point Clouds from the Start: Dynamic Removal Coupled with LIDAR-Inertial Odometry for Urban Scene

## 1.Introduction

This repository provides the implementation of our **Clean and Consistent MLS Point Clouds from the Start: Dynamic Removal Coupled with LIDAR-Inertial Odometry for Urban Scene**, which improves pose estimation and mapping accuracy in dynamic urban environments. The system is model-driven, voxel-free, and supports seamless integration with state-of-the-art LIO frameworks.


<p align="center">
  <img src="demo1.gif" alt="Demo Example 1" width="100%" />
</p>


### **1.1 Related paper**

✨ Our related papers has been submitted to "XX  Journal".

🚀 The source code will be released once our paper is accepted. Please stay tuned!

### **1.2 Related video**

Our accompanying videos are now available on **YouTube** (click below images to open) and [**Bilibili**](https://www.bilibili.com/video/123).

<div align="center">
<a href="https://www.youtube.com/123" target="_blank"><img src="img/cover.bmp" alt="video" width="60%" /></a>
</div>


## 2. Prerequisites

<p align="center">
  <img src="https://img.shields.io/badge/Ubuntu-20.04-orange?logo=ubuntu" />
  <img src="https://img.shields.io/badge/ROS-Noetic-blue?logo=ros" />
  <img src="https://img.shields.io/badge/PCL-≥1.8-green" />
  <img src="https://img.shields.io/badge/Eigen-≥3.3.4-yellow" />
  <img src="https://img.shields.io/badge/Livox-Driver-lightgrey" />
  <img src="https://img.shields.io/badge/TBB-Required-critical" />
</p>

### 2.1 Ubuntu & ROS
- **Ubuntu**: 20.04  
- **ROS**: Noetic  
  - Installation guide: [ROS Installation](http://wiki.ros.org/ROS/Installation)  

### 2.2 PCL & Eigen
- **PCL** ≥ 1.8  
`sudo apt install libpcl-dev`

- **Eigen**   ≥ 3.3.4

`sudo apt install libeigen3-dev`

### 2.3 **livox_ros_driver**

Follow [livox_ros_driver Installation](https://github.com/Livox-SDK/livox_ros_driver).


### 2.4 TBB

Follow [[TBB Installation](https://solarianprogrammer.com/2019/05/09/cpp-17-stl-parallel-algorithms-gcc-intel-tbb-linux-macos/)] (**Note:** change the gcc-9.1/g++-9.1 to gcc-9/g++-9)


## 2. Build

## 3. Directly run

## 4. Rosbag Example
### 4.1 Public Dataset

The City Datasets were utilized for the evaluation and ablation study of [MA-LIO](http://arxiv.org/abs/2305.16792). This dataset was collected in urban environments using a car, exhibiting high velocity, dynamic objects, numerous rotations with U-turns, and tunnels. The dataset was acquired using three LiDAR sensors (Livox Avia, Livox Tele, and OS2-128) and a 100Hz IMU. 

The KA-Urban Datasets were utilized for the evaluation and ablation study of [LiLi-OM](https://github.com/KIT-ISAS/lili-om)  This dataset was collected in urban environments using a bicycle, exhibiting high vibrations and dynamic objects. The datasets recorded by Livox Horizon (10 Hz) and Xsens MTi-670 (200 Hz). 

### 4.2 Private Dataset

We built a MLS collection system, which integrates a Livox HAP solid-state LiDAR, a high-precision IMU, multiple monocular RGB cameras, and a tightly coupled GNSS/IMU navigation system for generating ground-truth poses. To achieve accurate temporal alignment among all sensors, precision time protocol was adopted, ensuring nanosecond-level synchronization between LiDAR, IMU, and GNSS data.

The four private datasets were collected in Shanghai, China, across four urban regions, each containing diverse dynamic activity patterns. The recorded routes (Private\_01 to Private\_04) span between several hundred meters and over one kilometer. These areas were intentionally selected to capture high scene dynamics, including moving cars, pedestrians, and bicyclists under natural urban conditions. 


### Acknowledgements 


### License 
The source code is released under [GPLv2](http://www.gnu.org/licenses/) license.


