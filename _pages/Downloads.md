---
layout: about
permalink: /Downloads/
title: Downloads
description: On this page, you can download the benchmark data as rosbag or use our toolbox to select data topics you are interested in to create customized data.
nav: true
nav_order: 5
horizontal: true

---

## All sequences:

- <span style="font-size: 25px;">[All Indoor Sequences <--- Click to download](/cear/Downloads/indoorsequence/)</span>
- <span style="font-size: 25px;">[All Outdoor Sequences <--- Click to download](/cear/Downloads/outdoorsequence/)</span>
- <span style="font-size: 25px;">[All Backflip Sequences <--- Click to download](/cear/Downloads/backflipsequence/)</span>

---

**Data Structure:**

Event: event_*.aedat4   * represents the type of event camera

IMU: vectornav.txt   timestamp(us) gx(rad/s) gy(rad/s) gz(rad/s) ax(m/s^2) ay(m/s^2) az(m/s^2) magx magy magz qw qx qy qz

RealSense: realsense_timestamp.txt    timestamp(us)_depth_rgb.png timestamp_depth_event.png timestamp_rgb.png ...

LiDAR: lidar.bag    type: sensor_msgs/PointCloud2 topic: /velodyne_points

MoCap: MoCap.txt or FasterLIO.txt    timestamp(s) x y z qx qy qz qw

Joint: mini_cheetah_joint.txt    timestamp(us) FrontRight(abd hip knee) FrontLeft(abd hip knee) HindRight(abd hip knee) HindLeft(abd hip knee)  All in rad unit

*raw_rgb* stores unprocessed RGB images from RealSense camera and *rgb* folder stores processed (smoothed) RGB images. *raw_depth* stores depth images in depth camera's frame and *depth* folder stores projected depth images in RGB and event cameras frame.


---

Note: All ground-truth poses have been **synchronized** with the event camera's clock source. These ground-truth poses are represented in MoCap frame (obtained by OptiTrack) or LiDAR frames (obtained by FasterLIO). Other sensors' data is **not synchronized**, time offset parameters are [here](/EAGLE/Calibration/).

We also provide utils tools to convert from our data to ROS bag format: [here](https://github.com/DARoSLab/eagle_dataset_utils)

---


### Sensors for each sequence

|                                | DAVIS346 Event Camera | DVXplorer Event Camera | LiDAR | RGB-D Camera, IMU, Joint Encoders |
| ------------------------------ | --------------------- | ---------------------- | ----- | --------------------------------- |
| Indoor sequences               | ❌                     | ✔️                      | ✔️     | ✔️                                 |
| Outdoor sequences except for X | ✔️                     | ❌                      | ✔️     | ✔️                                 |
| Outdoor sequences X            | ❌                     | ✔️                      | ✔️     | ✔️                                 |
| Backflip sequences             | ❌                     | ✔️                      | ❌     | ✔️                                 |

* X represents around-building_day_comb, between-buildings_day_comb, downtown1_day_comb, downtown1_day_trot, downtown2_day_comb, downtown2_day_trot, forest_day_comb, forest_day_trot, grass1_day_comb, grass1_day_trot, grass1_night_comb, grass1_night_trot, parking-lot1_day_comb, parking-lot1_day_trot, parking-lot1_night_comb, parking-lot1_night_trot, residential-area_day_comb, residential-area_day_trot sequences.

|                                |       Sequence           |         Challenge      |Length  | 
| ------------------------------ |  ---------------------   | ---------------------- | -----  |
| Indoor sequences               | lab1_trot                | Slip                   |65m/159s | 
| Indoor sequences               | lab1_comb                | Slip                   |82m/245s | 
| Indoor sequences               | lab1_hdr_trot            | HDR, Slip              |66m/175s | 
| Indoor sequences               | lab1_hdr_comb            | Slip                   |81m/217s |  
| Indoor sequences               | classroom_trot           | Slip                   |28m/88s  | 
| Indoor sequences               | classroom_comb           | Slip                   |41m/134s | 
| Indoor sequences               | classroom_hdr_trot       | HDR, Slip              |28m/79s  | 
| Indoor sequences               | classroom_hdr_comb       | HDR, Slip              |41m/137s | 
| Indoor sequences               | classroom_blinking_trot  | Blinking, Slip         |28m/81s  | 
| Indoor sequences               | classroom_blinking_comb  | Blinking, Slip         |39m/122s | 
| Indoor sequences               | CS_building_3rdfloor_trot| Slip                   |211m/418s| 
| Indoor sequences               | CS_building_3rdfloor_comb| Slip                   |287m/587s| 
| Indoor sequences               | home1_trot               |                        |37m/111s | 
| Indoor sequences               | home1_comb               |                        |48m/143s | 
| Indoor sequences               | home2_trot               |                        |35m/120s | 
| Indoor sequences               | home2_comb               |                        |44m/155s | 
| Indoor sequences               | learning_center_trot     | Slip                   |140m/242s| 
| Indoor sequences               | learning_center_comb     | Slip                   |157m/350s| 
| Indoor sequences               | kitchen_trot             |                        |22m/85s  | 
| Indoor sequences               | kitchen_comb             |                        |31m/111s | 
| Indoor sequences               | kitchen_hdr_trot         | HDR                    |23m/91s  | 
| Indoor sequences               | kitchen_hdr_comb         | HDR                    |35m/112s | 
| Indoor sequences               | classroom_blinking_trot  | Blinking               |22m/93s  | 
| Indoor sequences               | classroom_blinking_comb  | Blinking               |36m/118s | 
| Indoor sequences               | LGRC_building_3rdfloor_trot| Slip                   |190m/384s| 
| Indoor sequences               | LGRC_building_3rdfloor_comb| Slip                   |255m/509s| 
| Indoor sequences               | lab2_trot                | Slip                   |44m/131s| 
| Indoor sequences               | lab2_comb                | Slip                   |56m/183s | 
| Indoor sequences               | lab2_hdr_trot            | HDR, Slip              |44m/120s | 
| Indoor sequences               | lab2_hdr_comb            | Slip                   |53m/167s |  
| Indoor sequences               |dining_hall_trot| Dyn                  |199m/341s| 
| Indoor sequences               | dining_hall_comb| Dyn                   |224m/471s| 
| Indoor sequences               | mocap_env1_trot           | Slip                   |32m/102s  | 
| Indoor sequences               | mocap_env1_comb           | Slip                   |54m/170s | 
| Indoor sequences               | mocap_dark_env1_trot           | Dark, Slip                  |33m/108s  | 
| Indoor sequences               | mocap_dark_env1_comb           | Dark, Slip                  |51/155s | 
| Indoor sequences               | mocap_blinking_env1_trot           | Blinking, Slip                  |34m/93s  | 
| Indoor sequences               | mocap_blinking_env1_comb           | Blinking, Slip                  |43m/122s | 
| Indoor sequences               | mocap_env2_trot           | Slip                   |31m/100s  | 
| Indoor sequences               | mocap_env2_comb           | Slip                   |47m/133s | 
| Indoor sequences               | mocap_dark_env2_trot           | Dark, Slip                  |32m/120s  | 
| Indoor sequences               | mocap_dark_env2_comb           | Dark, Slip                  |46/141s | 
| Indoor sequences               | mocap_blinking_env2_trot           | Blinking, Slip                  |31m/118s  | 
| Indoor sequences               | mocap_blinking_env2_comb           | Blinking, Slip                  |44m/131s | 
| Indoor sequences               | mocap_env3_trot           | Slip                   |31m/118s  | 
| Indoor sequences               | mocap_env3_comb           | Slip                   |51m/158s | 
| Indoor sequences               | mocap_dark_env3_trot           | Dark, Slip                  |31m/110s  | 
| Indoor sequences               | mocap_dark_env3_comb           | Dark, Slip                  |54/178s | 
| Indoor sequences               | mocap_blinking_env3_trot           | Blinking, Slip                  |31m/121s  | 
| Indoor sequences               | mocap_blinking_env3_comb           | Blinking, Slip                  |49m/147s | 
| Outdoor sequences              |around_building_day_trot | Dyn, Sun                  |422m/564s| 
| Outdoor sequences              |around_building_day_comb | Dyn                 |414m/469s| 
| Outdoor sequences              |around_building_night_trot | Dark                 |387m/366s| 
| Outdoor sequences              |around_building_night_comb | Dark                 |422m/564s| 
| Outdoor sequences              |between_building_day_trot | Sun                  |155m/200s| 
| Outdoor sequences              |between_building_day_comb | Sun                 |414m/469s| 
| Outdoor sequences              |between_building_night_trot | Dark                 |156m/193s| 
| Outdoor sequences              |between_building_night_comb | Dark                 |169m/282s| 
| Outdoor sequences              |downtown1_day_trot | Dark, Dyn                 |241m/296s| 
| Outdoor sequences              |downtown1_day_comb | Dyn                  |269m/473s| 
| Outdoor sequences              |downtown1_night_trot |  Dark, Dyn                |243m/282s| 
| Outdoor sequences              |downtown1_night_comb |  Dark, Dyn                 |266m/424s| 
| Outdoor sequences              |downtown2_day_trot | Dark, Dyn                 |187m/272s| 
| Outdoor sequences              |downtown2_day_comb | Dyn                  |190m/320s| 
| Outdoor sequences              |downtown2_night_trot |  Dark, Dyn                |174m/196s| 
| Outdoor sequences              |downtown2_night_comb |  Dark, Dyn                 |199m/451s| 
| Outdoor sequences              |forest_day_trot | Slip                |220m/249s| 
| Outdoor sequences              |forest_day_comb | Slip                |230m/321s| 
| Outdoor sequences              |forest_night_trot |  Slip                |213m/270s| 
| Outdoor sequences              |forest_night_comb |  Slip                 |236m/376s| 
| Outdoor sequences              |grass2_day_trot | Feat, Sun, Slip                 |261m/387s| 
| Outdoor sequences              |grass2_day_comb | Feat, Sun, Slip                 |285m/533s| 
| Outdoor sequences              |grass2_night_trot |  Feat, Slip               |268m/292s| 
| Outdoor sequences              |grass2_night_comb |  Feat, Slip                 |287m/395s| 
| Outdoor sequences              |parking_lot2_day_trot | Feat               |460m/436s| 
| Outdoor sequences              |parking_lot2_day_comb | Feat               |486m/609s| 
| Outdoor sequences              |parking_lot2_night_trot |  Dark, Feat               |461m/379s| 
| Outdoor sequences              |parking_lot2_night_comb |  Dark, Feat, Fog                 |508m/820s| 
| Outdoor sequences              |residential_area_day_trot |              |621m/701s| 
| Outdoor sequences              |residential_area_day_comb |              |655m/792s| 
| Outdoor sequences              |residential_area_night_trot |  Dark, Dyn               |655m/792s| 
| Outdoor sequences              |residential_area_night_comb |  Dark,  Dyn                 |655m/792s| 
| Outdoor sequences              |sidewalk1_area_day_trot |              |133m/127s| 
| Outdoor sequences              |sidewalk1_area_day_comb |              |143m/180s| 
| Outdoor sequences              |sidewalk1_area_night_trot |  Dark              |137m/163s| 
| Outdoor sequences              |sidewalk1_area_night_comb |  Dark                |142m/192s| 
| Outdoor sequences              |sidewalk2_area_day_trot |              |579m/610s| 
| Outdoor sequences              |sidewalk2_area_day_comb |              |682m/1127s| 
| Outdoor sequences              |sidewalk2_area_night_trot |  Dark              |724m/646s| 
| Outdoor sequences              |sidewalk2_area_night_comb |  Dark, Frog                |687m/1114s| 
| Backflip             |env1_backflip1 |  Ag                 |11m/111s| 
| Backflip             |env1_backflip2 |  Ag                 |11m/123s| 
| Backflip             |env2_backflip1 |  Ag                 |10m/90s| 
| Backflip             |env2_backflip2 |  Ag                 |10m/88s| 
| Backflip             |env3_backflip1 |  Ag                 |11m/119s| 
| Backflip             |env3_backflip2 |  Ag                 |11m/125s|
| Backflip             |env4_backflip1 |  Ag                 |11m/97s| 
| Backflip             |env4_backflip2 |  Ag                 |11m/105s|
| Backflip             |env5_backflip1 |  Ag                 |11m/104s| 
| Backflip             |env5_backflip2 |  Ag                 |11m/76s| 
| Backflip             |env6_backflip1 |  Ag                 |10m/82s| 
| Backflip             |env6_backflip2 |  Ag                 |10m/80s| 
| Backflip             |env7_backflip1 |  Ag                 |11m/84s| 
| Backflip             |env7_backflip2 |  Ag                 |11m/90s|
| Backflip             |env8_backflip1 |  Ag                 |11m/78s| 
| Backflip             |env8_backflip2 |  Ag                 |11m/79s|

<script>
  document.addEventListener('DOMContentLoaded', function() {
    var video = document.getElementById('myVideo');

    video.addEventListener('ended', function() {
      this.currentTime = 0;
      this.play();
    });
  });
</script>


### Indoor sequence example
Indoor sequences were collected in 13 diverse environments under a range of lighting conditions: well-lit, dark, HDR, and blinking. \*_trot means a trot-only gait and *_comb means a combination of trotting, bounding, and pronking gaits.

<div style="display: flex; flex-wrap: wrap;">
    <!-- Video 1 -->
    <div style="flex: 32%; text-align: center;">
       <h5 style="margin-bottom: 10px;"> mocap_env1_trot
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/indoor/mocap_env1_trot.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 2 -->
    <div style="flex: 32%; text-align: center;">
        <h5 style="margin-bottom: 10px;">mocap_env1_dark_trot 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/indoor/mocap_env1_dark_trot.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 3 -->
    <div style="flex: 32%; text-align: center;">
        <h5 style="margin-bottom: 10px;">mocap_env1_blinking_trot 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/indoor/mocap_env1_blinking_trot.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 4 -->
    <div style="flex: 32%; text-align: center;">
        <h5 style="margin-bottom: 10px;">mocap_env1_comb 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/indoor/mocap_env1_comb.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 5 -->
    <div style="flex: 32%; text-align: center;">
        <h5 style="margin-bottom: 10px;">mocap_env1_dark_comb 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/indoor/mocap_env1_dark_comb.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 6 -->
    <div style="flex: 32%; text-align: center;">
        <h5 style="margin-bottom: 10px;">mocap_env1_blinking_comb
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/indoor/mocap_env1_blinking_comb.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>
</div>

### Outdoor sequence example
The outdoor sequences were captured in 10 distinctive outdoor environments, with four sequences per environment. Each set of four sequences includes variations of two different sets of quadruped gaits (trot-only and combined gaits) under different periods of the day (daytime and nighttime).


<div style="display: flex; flex-wrap: wrap;">
    <!-- Video 1 -->
    <div style="flex: 40%; text-align: center;">
        <h5 style="margin-bottom: 10px;">between_buildings_day_trot 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/outdoor/between_buildings_day_trot.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 2 -->
    <div style="flex: 40%; text-align: center;">
        <h5 style="margin-bottom: 10px;">between_buildings_night_trot 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/outdoor/between_buildings_night_trot.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 3 -->
    <div style="flex: 40%; text-align: center;">
        <h5 style="margin-bottom: 10px;">between_buildings_day_comb 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/outdoor/between_buildings_day_comb.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 4 -->
    <div style="flex: 40%; text-align: center;">
        <h5 style="margin-bottom: 10px;">between_buildings_night_comb 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/outdoor/between_buildings_night_comb.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>
</div>

### Backflip sequence example

Backflip sequences were captured in 7 indoor environments and 1 outdoor environment, with two sequences in each environment.

<div style="display: flex; flex-wrap: wrap;">
    <!-- Video 1 -->
    <div style="flex: 32%; text-align: center;">
        <h5 style="margin-bottom: 10px;"> env1_backflip1
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/backflip/env1_backflip1.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 2 -->
    <div style="flex: 32%; text-align: center;">
        <h5 style="margin-bottom: 10px;"> env1_backflip2 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/backflip/env1_backflip2.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>
</div>
