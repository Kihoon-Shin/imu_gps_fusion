# Imu and Gps Fusion by ESKF
## Explain
- [https://blog.csdn.net/weixin_37835423/article/details/109452148](https://blog.csdn.net/weixin_37835423/article/details/109452148)
- [https://blog.csdn.net/weixin_37835423/article/details/109476346](https://blog.csdn.net/weixin_37835423/article/details/109476346)

## Requirements

- [ROS Kinetic](http://wiki.ros.org/kinetic/Installation/Ubuntu)
- Eigen3

## Reference Theory

- [Quaternion kinematics for error state kalman filter](http://www.iri.upc.edu/people/jsola/JoanSola/objectes/notes/kinematics.pdf)

## Used in

- [wgs_conversions]( https://github.com/gyjun0230/wgs_conversions ) for transform between coordinate in wgs frame and coordinate in enu frame

## Dataset

- https://lcas.lincoln.ac.uk/nextcloud/index.php/s/KfItDFgwwis5Xrk

## Test

```
roslaunch imu_gps_fusion imu_gps_fusion.launch
```

```
rosbag play *.bag --clock
```

## Result
![result](https://user-images.githubusercontent.com/82350419/232706594-36b1d094-ce2c-4bbf-b1ed-a4c4db61346f.png)

