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

&nbsp;<br>

---
### Data Structure

Below is the data structure for each sequence:

- **Event:**
  - `event_*.aedat4` (* represents the type of event camera)

- **IMU:**
  - `vectornav.txt`
    - `timestamp(us) gx(rad/s) gy(rad/s) gz(rad/s) ax(m/s^2) ay(m/s^2) az(m/s^2) magx magy magz qw qx qy qz`

- **RealSense:**
  - `realsense_timestamp.txt`
    - `timestamp(us)_depth_rgb.png timestamp_depth_event.png timestamp_rgb.png …`

- **LiDAR:**
  - `lidar.bag`
    - Type: `sensor_msgs/PointCloud2`
    - Topic: `/velodyne_points`

- **MoCap:**
  - `MoCap.txt` or `FasterLIO.txt`
    - `timestamp(s) x y z qx qy qz qw`

- **Joint:**
  - `mini_cheetah_joint.txt`
    - `timestamp(us) FrontRight(abd hip knee) FrontLeft(abd hip knee) HindRight(abd hip knee) HindLeft(abd hip knee)` All in rad unit

- **Raw and Processed Data:**
  - `raw_rgb` stores unprocessed RGB images from RealSense camera.
  - `rgb` folder stores processed (smoothed/noise-free) RGB images.
  - `raw_depth` stores depth images in **depth** camera’s frame.
  - `depth` folder stores projected depth images in **RGB** and **event** cameras frame.


&nbsp;<br>

---
### Sensors for each sequence

|                                | DAVIS346 Event Camera | DVXplorer Event Camera | LiDAR | RGB-D Camera, IMU, Joint Encoders |
| ------------------------------ | --------------------- | ---------------------- | ----- | --------------------------------- |
| Indoor sequences               | ❌                     | ✔️                      | ✔️     | ✔️                                 |
| Outdoor sequences except for X | ✔️                     | ❌                      | ✔️     | ✔️                                 |
| Outdoor sequences X            | ❌                     | ✔️                      | ✔️     | ✔️                                 |
| Backflip sequences             | ❌                     | ✔️                      | ❌     | ✔️                                 |

* X represents around-building_day_comb, between-buildings_day_comb, downtown1_day_comb, downtown1_day_trot, downtown2_day_comb, downtown2_day_trot, forest_day_comb, forest_day_trot, grass1_day_comb, grass1_day_trot, grass1_night_comb, grass1_night_trot, parking-lot1_day_comb, parking-lot1_day_trot, parking-lot1_night_comb, parking-lot1_night_trot, residential-area_day_comb, residential-area_day_trot sequences.

&nbsp;<br>

---
### Challenges for each seqeuence

We have also identified and categorized the challenging features in the dataset as follows: Agile locomotion (Ag), Dynamic objects (Dyn), High dynamic range (HDR), Darkness (Dark), Direct sunlight (Sun), Blinking light (Blink), Slippery ground (Slip), Featureless regions (Feat), and Foggy weather (Fog)

- <span style="font-size: 21px;">[Click to check challenges for each sequence](/cear/Downloads/challenges/)</span>


<script>
  document.addEventListener('DOMContentLoaded', function() {
    var video = document.getElementById('myVideo');

    video.addEventListener('ended', function() {
      this.currentTime = 0;
      this.play();
    });
  });
</script>

&nbsp;<br>

---
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

&nbsp;<br>

---
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

&nbsp;<br>

---
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
