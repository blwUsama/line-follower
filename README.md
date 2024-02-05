<h2>University Project - Line Follower</h2>
Assembled a robot capable of autonomously following a predefined path.<br>
This project was developed within a 3-person team, "Robo Putrezitul", along with <a href="https://github.com/Teo0o0">@Teo0o0</a> and <a href="https://github.com/criss505">@criss505</a>.<br><br><details>
<summary>Project details</summary>
This project integrates sensors, motors, and a control algorithm to enable navigating along the track marked by a black line.<br>
Our robot completed the final track in 20.5 seconds, slightly over the maximum-grade threshold (20 seconds).<br>
  
<h3>Components</h3>
  1.Arduino Uno<br>
  2.Breadboard (a small one)<br>
  3.Power source (LiPo battery)<br>
  4.QTR reflectance sensor<br>
  5.2 Wheels<br>
  6.2 DC motors<br>
  7.Ball caster<br>
  8.Wires<br>
  9.Zip-ties<br>
  10.Chassis (created with foamcore)<br>

<h3>Main Functionalities</h3>
  Line Detection - The sensors continuously monitor the surface and process the data to determine the robot's position relative to the line.<br>
  Control Algorithm - The code is implemented to make decisions regarding direction based on the line sensor data (through adjusting motor speeds).<br>
  Autonomous Navigation - The robot makes real-time adjustments to navigate through curves and stay on track.<br>

<h3>Chassis Design</h3>
The chassis was created out of foamboard, with a few points in mind when designed.<br>
Complex forms were avoided to improve stability and durableness, while securing the other pieces attached.<br>
The sensors were placed in front, along with the ball caster, to facilitate the detection of incoming path, while the motor-controlled wheels were placed at the back for more control when making turns.<br>
We placed the LiPo battery (heaviest piece) on the lowest level in the center of the chassis and the breadboard above it, to lower the center of gravity.<br>
When fixing the battery, we used a pin to hold it in place to ensure a smooth change when changing it to a charged one is needed.<br>


<h3>Calibration</h3>
The robot is able to self-calibrate, not needing manual handling when being turned on.<br>
This is done through the robot turning left-right before starting to follow the line.<br>

<h3>Parameter Tuning</h3>
The PID values were low or 0 at first, until we experimented with several sets to find the optimal numbers for our setup.<br>
The main traits we looked at when evaluating the parameter values were the sharpness of the turns and the shaking on straight paths.<br>
The final values were kp=15, ki=0, kd=7.<br>


</details>

-> <a href="https://youtu.be/uPR8K8UPLq4">video of the best lap</a>
