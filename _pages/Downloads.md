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

- <span style="font-size: 22px;">[All Indoor Sequences](/EAGLE/Downloads/indoorsequence/)</span>
- <span style="font-size: 22px;">[All Outdoor Sequences](/EAGLE/Downloads/outdoorsequence/)</span>
- <span style="font-size: 22px;">[All Backflip Sequences](/EAGLE/Downloads/backflipsequence/)</span>


<script>
  document.addEventListener('DOMContentLoaded', function() {
    var video = document.getElementById('myVideo');

    video.addEventListener('ended', function() {
      this.currentTime = 0;
      this.play();
    });
  });
</script>

#### Indoor sequences were collected in 13 diverse environments under a range of lighting conditions: well-lit, dark, HDR, and blinking.

#### The outdoor sequences were captured in 10 distinctive outdoor environments, with four sequences per environment. Each set of four sequences includes variations of two different sets of quadruped gaits (trot-only and combined gaits) under different periods of the day (daytime and nighttime)

#### \*_trot means a trot-only gait and *_comb means a combination of trotting, bounding, and pronking gaits.


### Indoor sequence example

<div style="display: flex; flex-wrap: wrap;">
    <!-- Video 1 -->
    <div style="flex: 32%; text-align: center;">
        <h5 style="margin-bottom: 10px;">mocap_env1_trot 
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



<div style="display: flex; flex-wrap: wrap;">
    <!-- Video 1 -->
    <div style="flex: 48%; text-align: center;">
        <h5 style="margin-bottom: 10px;">between_buildings_day_trot 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/outdoor/between_buildings_day_trot" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 2 -->
    <div style="flex: 48%; text-align: center;">
        <h5 style="margin-bottom: 10px;">between_buildings_night_trot 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/outdoor/between_buildings_night_trot.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 3 -->
    <div style="flex: 48%; text-align: center;">
        <h5 style="margin-bottom: 10px;">between_buildings_day_comb 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/outdoor/between_buildings_day_comb.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 4 -->
    <div style="flex: 48%; text-align: center;">
        <h5 style="margin-bottom: 10px;">between_buildings_night_comb 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/outdoor/between_buildings_night_comb" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>
</div>

### Backflip sequence example


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
