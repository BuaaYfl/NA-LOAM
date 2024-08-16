# NA-LOAM
Source code of NA-LOAM: Normal-based Adaptive LiDAR Odometry and Mapping


The code and relavent materials will be uploaded upon acceptance of the paper.


## 1. Prerequisites
### 1.1 **Ubuntu** and **ROS**
**Ubuntu >= 18.04**

For **Ubuntu 18.04 or higher**, the **default** PCL and Eigen is enough for NA-LOAM to work normally.

[//]: # ()
[//]: # (ROS    >= Melodic. [ROS Installation]&#40;http://wiki.ros.org/ROS/Installation&#41;)

### 1.2 Ground-FALS Normal Estimator
Compile follow [Ring FALS normal estimator](https://github.com/tiev-tongji/RingFalsNormal).

#### KITTI Dataset
Both the frequency of images and LiDAR point clouds of  [*KITTI-Odometry*](https://www.cvlibs.net/datasets/kitti/eval_odometry.php) are 10 Hz, while they are strictly one-to-one. In addition, the motion distortion of LiDAR pont cluods have been calibrated in advance, therefore, users do not need to consider the effect of motion distortion when evaluation on *KITTI-Odometry*. Users can directly utilize the [*KITTI-Odometry to ROS bag*](https://github.com/ZikangYuan/kitti2bag) tool to convert data of *KITTI odometry* to ROS bag format.
