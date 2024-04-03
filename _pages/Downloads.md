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
        <h5 style="margin-bottom: 10px;">mocap_env1_trot 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/outdoor/between_buildings_day_trot" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 2 -->
    <div style="flex: 48%; text-align: center;">
        <h5 style="margin-bottom: 10px;">mocap_env1_dark_trot 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/outdoor/between_buildings_night_trot.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 3 -->
    <div style="flex: 48%; text-align: center;">
        <h5 style="margin-bottom: 10px;">mocap_env1_blinking_trot 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/outdoor/between_buildings_day_comb.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>

    <!-- Video 4 -->
    <div style="flex: 48%; text-align: center;">
        <h5 style="margin-bottom: 10px;">mocap_env1_comb 
        </h5>
        <video style="width: 100%; height: auto;" autoplay muted loop>
            <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/outdoor/between_buildings_night_comb" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>
</div>

### Backflip sequence example


<div style="margin-bottom: -15mm; z-index: 10; position: relative;">
  <h5>env1_backflip1 &nbsp;&nbsp;&nbsp;&nbsp; <a href="https://drive.google.com/file/d/18gmQA3DuIlzIMyYaMtTWxYduX91uZTaV/view?usp=drive_link">Data(4.06GB)</a> &nbsp;&nbsp;&nbsp;&nbsp; GT_Pose</h5>
</div>
<div style="margin-top: -15mm;">
  <video id="myVideo" width="640" height="360" autoplay muted loop>
    <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/backflip/env1_backflip1.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

<div style="margin-bottom: -15mm; z-index: 10; position: relative;">
  <h5>env1_backflip2 &nbsp;&nbsp;&nbsp;&nbsp; <a href="https://drive.google.com/file/d/1QatyjhJS9WaR0ChtVFFtfIaQFkD9CVLy/view?usp=drive_link">Data(3.36GB)</a> &nbsp;&nbsp;&nbsp;&nbsp; GT_Pose</h5>
</div>
<div style="margin-top: -15mm;">
  <video id="myVideo" width="640" height="360" autoplay muted loop>
    <source src="https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/video/backflip/env1_backflip2.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>


