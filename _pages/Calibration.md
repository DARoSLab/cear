---
layout: page
title: Calibration
permalink: /Calibration/
description:
nav: true
nav_order: 4  
horizontal: false
---


---

Note: All ground-truth poses have been **synchronized** with the event camera's clock source. These ground-truth poses are represented in MoCap frame (obtained by OptiTrack) or LiDAR frames (obtained by FasterLIO). Other sensors' data is **not synchronized**, time offset parameters are [here](/EAGLE/Calibration/).

We also provide utils tools to convert from our data to ROS bag format: [here](https://github.com/DARoSLab/eagle_dataset_utils)


---
## Time offset parameters (second)

EventCamera: 0.0

MiniCheetahJoint: 0.004611

VectorNav: -0.004012

RealSense (depth camera): 0.004611

Velodyne: 0.003044

E.g. Time_event = Time_vectornav - 0.004012

---
## Intrinsic parameters

##### DAVIS346 event camera: &nbsp;&nbsp;&nbsp;&nbsp; [result](https://drive.google.com/file/d/1RaBTbBw7ZbvR-TW1HlMCD-Q7zRDQqgjo/view?usp=drive_link)

##### DVXplorer Lite event camera: &nbsp;&nbsp;&nbsp;&nbsp; [result](https://drive.google.com/file/d/1zG2fZABrEVrqjUQ_EaikEnmEMWwqjdj-/view?usp=drive_link)

##### RealSense RGBD camera: &nbsp;&nbsp;&nbsp;&nbsp; [result](https://drive.google.com/file/d/18vLEDh_gjX25PapgfI6racGMKtI7e5Sw/view?usp=drive_link)

##### VectorNav IMU: &nbsp;&nbsp;&nbsp;&nbsp; [result](https://drive.google.com/file/d/1y6c6SAr_qaBWx0XAr2pgwvVUuAN-pXSp/view?usp=drive_link)



## Extrinsic parameters
---
##### Event IMU: &nbsp;&nbsp;&nbsp;&nbsp; [result](https://drive.google.com/file/d/1LLyt4-r7N6z3lC2m0G1IFmjnEV2VwUB9/view?usp=drive_link)

##### Event RGB: &nbsp;&nbsp;&nbsp;&nbsp; [result](https://drive.google.com/file/d/1sAij16MgFDjAzZAkVyfcUnNn_sH6cOpN/view?usp=drive_link)

##### Event LiDAR: &nbsp;&nbsp;&nbsp;&nbsp; [result](https://drive.google.com/file/d/13E0TcEdK7u-YI4HmLRvHlZMndmbR9B7o/view?usp=drive_link)

##### RGB Depth: &nbsp;&nbsp;&nbsp;&nbsp; [result](https://drive.google.com/file/d/18xIn3x1EH-1tZ43yl0fJzC9MNRfRLt40/view?usp=drive_link)

##### RGB Robot: &nbsp;&nbsp;&nbsp;&nbsp; [result](https://drive.google.com/file/d/1Vlr01SkgorLVqzUNas3tWOe4E1WJ8HK8/view?usp=drive_link)

##### RGB Marker: &nbsp;&nbsp;&nbsp;&nbsp; [result](https://drive.google.com/file/d/11s58CDnDjQP7XAzR9B6eRVkaSElQPuoQ/view?usp=drive_link)

##### Robot Links: &nbsp;&nbsp;&nbsp;&nbsp; [result](https://drive.google.com/file/d/1b-tvjlJe6tQa-d5bC0vY5_CTV81R7IHq/view?usp=drive_link)
