---
layout: page
permalink: /Download/
title: Download
description: On this page, you can download the benchmark data as rosbag or use our toolbox to select data topics you are interested in to create customized data.
nav: true
nav_order: 5
display_categories: [around_building_day, around_building_night, between_buildings_day, 
between_buildings_night, downtown1_day, downtown1_nignt, downtown2_day, downtown2_night, forest_day, forest_night, grass_day, grass_night, 
parking_lot_day, parking_lot_night, resident_area_day, resident_area_night, sidewalk2_day, sidewalk2_night, sidewalk1_day, sidewalk1_night]
display_categories2: [dataset3, dataset4]
horizontal: true
---
## Indoor scequences
---
##### mocap_env1_trot &nbsp;&nbsp;&nbsp;&nbsp; [Data(4.95GB)](https://drive.google.com/file/d/1BGD_9tUYrxLmVhRj3dp_Tz5M5Fj--__2/view?usp=drive_link) &nbsp;&nbsp;&nbsp;&nbsp; GT_Pose

![Figure 1](https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/img/download/arrow_elevator_up_runner_md_nwm_v2.gif) ![Figure 2](https://raw.githubusercontent.com/DARoSLab/EAGLE/main/assets/img/download/arrow_elevator_up_runner_md_nwm_v2.gif)

##### mocap_env1_trot    Data(4.95GB)    GT_Pose

##### mocap_env1_trot    Data(4.95GB)    GT_Pose

##### mocap_env1_trot    Data(4.95GB)    GT_Pose

##### mocap_env1_trot    Data(4.95GB)    GT_Pose

##### mocap_env1_trot    Data(4.95GB)    GT_Pose

##### mocap_env1_trot    Data(4.95GB)    GT_Pose

---
## Outdoor scequences
---
##### around_building_day_trot    Data(22.57GB)    GT_Pose





---
## Backflip scequences
---
##### To be done



<!-- pages/projects.md -->
<div class="projects">
  <div style="text-align: center; font-size: 24px;">
    <p>Indoor</p>
  </div>

{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>


<!-- pages/projects.md -->
<div class="projects">
  <div style="text-align: center; font-size: 24px;">
    <p>Outdoor</p>
  </div>

{%- if site.enable_project_categories and page.display_categories2 %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories2 %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>

