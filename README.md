
Sonar Based SLAMC (Simultaneous Localization, Mapping and Classification)
------------------------
<p align="center">
<img src="http://i.imgur.com/NUavBHa.png" height="400" width=auto>
</p>

* Still working on it<br><br>

### Abstract ###
For the last 52 million years bats use echo-location for navigation, localization and classification purpose. Agrirobot, innovative approach to agricultural technology using bio-inspired SONAR, based on similar acoustic signals that bats transmit we can apply different methods for solving the well-known SLAM problem.
Focusing at the on the robotic orientation aspects of the Agrirobot, developing a SONAR based method for robotic- mapping, obstacle avoidance and path planning in a greenhouse or an orchard. This will allow the yield-assessment robot to autonomously navigate in the greenhouse or orchard based on bio-SONAR only. Such an ability is an essential step on the way to developing a fully automatic yield assessment approach which will be far cheaper and more accurate than the all measures which are currently in use.

### Thesis Outline ###
* Introduction
* Equipment

* Passive Sonar Localization (BAT-GPS)
    Basics of high frequency chirp signals
    Transmit, receive signal using independent systems
    Cross correlation between signals
    TDOA – Time Difference Of Arrival Methods (Chan, Foy, Grid-Search)

* Active Sonar Navigation
    Construct 2D map base on acoustic signals
    Advantages of ultrasonic signals to “See-Trough” objects

* Path Planning and Classification
    Classification of signals using Neural Network - TensorFlow
    Path planning based ROS Navigation Stacks
    Decision making - Cul-de-Sac

### Hardware ###
* Komodo Robot Platform
* DJI Ronin Gimbal + Custom Control Board
link: <br> https://github.com/Itamare4/dji_ronin
* Speed of sound calibration
* Passive Localization Unit:<br>
    4x Avisoft Vifa Speaker<br>
    1x DAQ - Measurement Computing - USB-1608GX-2AO<br>
    1x Avisoft Bioacoustics CM16/CMPA40-5V - Omni microphone<br>
    1x Sony XM-GS4 <br>
    
* Front Sensing Unit:<br>
    1x Avisoft Vifa Speaker<br>
    1x DAQ - Measurement Computing - USB-1608GX-2AO<br>
    2x Avisoft Bioacoustics CM16/CMPA40-5V - Directional microphone<br>
    1x Sony XM-GS4 <br>
    1x Thermal Camera - Flir Ax5 <br>
    1x RGB Camera - uEye CP <br>
    1x Leica D410 <br>
<p align="center">
<img src="https://s2.postimg.org/4sfwmqti1/Front_Sensing_Unit.png">
</p>

### Software ###
* Ubuntu 14.04 LTS
* ROS Indigo


### Algorithm Architecture ###
<p align="center">
<img src="https://s1.postimg.org/r1yypslxr/Algorithm_Arch.png" height="400" width=auto>
</p>

### Publications & Citations ###
▪	Eliakim I., Yovel Y., Kosa G., “Acoustic Self-Localization for Mobile Robots” IPIN (Indoor Positioning Indoor Navigation) 2016, Madrid, Spain<br>
▪ Soon.

### About ###
Itamar Eliakim<br>
M.Sc Student Mechanical Engineering Faculty at Tel Aviv University, Israel<br>
Email - Itamare@gmail.com


