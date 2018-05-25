
Sonar Based SLAMC (Simultaneous Localization, Mapping and Classification)
------------------------
<p align="center">
<img src="http://i.imgur.com/NUavBHa.png" height="400" width=auto>
<img src="https://github.com/Itamare4/Thesis_private/raw/master/MD_Images/Robot_Back_GreenHouse.png?raw=true" height="400" width=auto>
</p>

### Contacts ###
Itamar Eliakim, Editor <br>
Dr. Yossi Yovel, Advisor <br>
Dr. Gabor Kosa, Advisor <br>

### Abstract ###
For the last 52 million years bats use echo-location for navigation, localization and classification purpose. Agrirobot, innovative approach to agricultural technology using bio-inspired SONAR, based on similar acoustic signals that bats transmit we can apply different methods for solving the well-known SLAM problem.
Focusing at the on the robotic orientation aspects of the Agrirobot, developing a SONAR based method for robotic- mapping, obstacle avoidance and path planning in a greenhouse or an orchard. This will allow the yield-assessment robot to autonomously navigate in the greenhouse or orchard based on bio-SONAR only. Such an ability is an essential step on the way to developing a fully automatic yield assessment approach which will be far cheaper and more accurate than the all measures which are currently in use.

### Thesis Outline ###
* Introduction<br>
* Hardware & Software <br>

* Passive Sonar Localization (BAT-GPS) <br>
    * Basics of high frequency chirp signals <br>
    * Transmit, receive signal using independent systems<br>
    * Cross correlation between signals<br>
    * TDOA – Time Difference Of Arrival Methods (Chan, Foy, Grid-Search)<br>

* Active Sonar Navigation<br>
    * Construct 2D map base on acoustic signals<br>
    * Iterative Obstacle Inflation<br>
    * Advantages of ultrasonic signals, use of one and two ears<br>

* Path Planning and Classification<br>
    * Classification of signals using Neural Network - TensorFlow<br>
    * Path planning based ROS Navigation Stacks<br>
    * Decision making - Cul-de-Sac<br>

### Hardware ###
* Komodo Robot Platform
* DJI Ronin Gimbal + Custom Control Board
link: <br> https://github.com/Itamare4/dji_ronin
* Speed of sound calibration
* Passive Localization Unit:<br>
    * 4x Avisoft Vifa Speaker<br>
    * 1x DAQ - Measurement Computing - USB-1608GX-2AO<br>
    * 1x Avisoft Bioacoustics CM16/CMPA40-5V - Omni microphone<br>
    * 1x Sony XM-GS4 <br>
<p align="center">
<img src="https://s1.postimg.org/lkh4hlq4f/Localization_Equipment.png">
</p>  <br>
* Front Sensing Unit:<br>
    * 1x Avisoft Vifa Speaker<br>
    * 1x DAQ - Measurement Computing - USB-1608GX-2AO<br>
    * 2x Avisoft Bioacoustics CM16/CMPA40-5V - Directional microphone<br>
    * 1x Sony XM-GS4 <br>
    * 1x Thermal Camera - Flir Ax5 <br>
    * 1x RGB Camera - uEye CP <br>
    * 1x Leica D410 <br>
<p align="center">
<img src="https://github.com/Itamare4/Thesis_private/raw/master/MD_Images/Front_Sensing_Unit.png?raw=true">
</p>

### Software ###
* Ubuntu 14.04 LTS
* ROS Indigo


### Algorithm Architecture ###
<p align="center">
<img src="https://github.com/Itamare4/Thesis_private/raw/master/MD_Images/Algorithm_Architecture.png?raw=true" height="400" width=auto>
</p>

### Experiments ###
Experiments done in 3 different locations: Robotics LAB - Wolfson Building, Tel Aviv University, first experiments done indoor mapping of the lab environment, mapping dimensions - (6m x 4m),  this set of experiments done based on one ear mapping, will explained below, at each point the robot collects chirp signals at 5 different angles,  [-90°,-45°,0°,45°,90°], second set of experiments done at pteridophytes greenhouse at Botanical Garden, Tel Aviv University, mapping dimensions (5m x 12m), mapping based on two ears(ITD), at each point the robot collects chirp signals at 3 different angles, (0,-60, 60). third set done at the palm greenhouse at Botanical Garden, Tel Aviv University, mapping dimensions (40m x 5m), data collections similar to experiments done at the pteridophytes greenhouse.

| [![Palm]()](https://github.com/Itamare4/Thesis_private/raw/master/MD_Images/Palm_EXP.jpg?raw=true)  | [![Pteridophytes]()](https://github.com/Itamare4/Thesis_private/raw/master/MD_Images/Pteridophytes_EXP.png?raw=true) | [![Wolfson]()](https://s2.postimg.org/3mv3murad/Wolfson_EXP.png) |
|:---:|:---:|:---:|
| Palm Greenhouse, Botanical Garden | Pteridophytes Greenhouse, Botanical Garden | Wolfson Building, Mechanical Engineering Faculty |

### Results ###
<p align="center">
<img src="https://s21.postimg.org/5t7uni16v/image.png" height="300"><br>Sonar Localization, Mapping and Classification, with 3 iteration of IOI, iterative obstacle inflation.<br>
link - https://github.com/Itamare4/ROS_smooth_map
</p>
<p align="center">
<img src="https://s1.postimg.org/3oyl0qd8v/image.png" height="150"><br>Palm Greenhouse Top View, Ground Truth Based on Aerial Footage Using DJI Phantom 4<br>
</p>

### Videos ###
[![SLAMC](http://img.youtube.com/vi/I9OVUKLDUHE/0.jpg)](http://www.youtube.com/watch?v=I9OVUKLDUHE "Sonar Based SLAMC(Simultaneous Localization Mapping and Classification) ")

### Photo Album ###
Photos from outdoor, indoor experiments are available on:<br>
link: 

### Publications & Citations ###
▪	Eliakim I., Yovel Y., Kosa G., “Acoustic Self-Localization for Mobile Robots” IPIN (Indoor Positioning Indoor Navigation) 2016, Madrid, Spain<br>
▪ Soon.

### About ###
Itamar Eliakim<br>
M.Sc Student Mechanical Engineering Faculty at Tel Aviv University, Israel<br>
Email - Itamare@gmail.com


