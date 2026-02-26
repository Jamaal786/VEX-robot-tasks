# VEX robot tasks

## 📌 Overview
This project involved developing the control software for a VEX robot to complete a seiries of tasks as part of a main mission. The robot was required to comply with competition rules while achieving objectives to maximise its overall score. My primary role was to develop code for controlling the robot's arm, enabling it to raise and lower as required. I also implmented the use of SONAR sensing to detect objects and stop a pre defined distance. I aided in refining the line following alogorithm to improve navigation reliability. I also drew up flowcharts of the main program and functions which helped with planning, debugging, and overall system organisation. 

## 🎯 Objectives
- Arm raised and lowered accuratey via P controller
- Robot stops certain distance away from blockage set at any distance away from payload
- Robot follows line accurately
  
## 🛠 Tools & Concepts Used
- C programming
- Concept of a PI controller
- SONAR Sensor Integration
- IR Sensor Line Following
- Encoder Feedback Control 

## 🔍 Methodology
#### Arm Function
The arm position was controlled using encoder feedback from the arm motor. Encoder counts were converted into angular position (degrees), which provided a more intuitive and precise way to define the required arm positions for payload pickup and drop-off. 
<br>

A proportional (P) controller was implemented to regulate the arm position. A proportional integral (PI) controller was not necessary, as the system did not need high positional precision and the arm operated within a relatively large acceptable range. The P controller provided sufficient responsiveness and stability while keeping the control implementation simple.

#### SONAR

The SONAR functionality utilised the built-in SONAR sensor on the VEX robotic to detect the distance between the robot and obstacles ahead. The measured distance was continuously monitored and used to determine when the robot should stop before reaching the blockade.
<br>

Through testing and adjustments, an appropriate stopping distance was determined to ensure reliable payload pickup. Once this distance was reached, a separate function was called to initiate the payload pick up sequence.

#### Line Following

The line-following function was initially developed by my lab partner. To assist with debugging and improvement, I reviewed the implementation and analysed the control logic independently to fully understand the system.<br>

After investigation, I determined that the core algorithm was functioning correctly. However, the infrared (IR) sensor threshold values required calibration. These values were refined through iterative testing to improve the robot’s ability to detect and follow the line.<br>

Although the final implementation achieved a working line following function, the system’s reliability was sensitive to the IR sensor calibration and environmental conditions. This highlighted the importance of proper sensor tuning and robustness in autonomous navigation systems. 

## 📊 Results
- All core functions were successfully implemented and integrated into the robot.
- The arm control and SONAR functions performed reliably and met the functional requirements for payload handling and obstacle detection.
- The line-following function was ultimately successful in enabling autonomous navigation. However, it required extensive calibration and remained less robust than the other subsystems. 

## 📸 Project Images
The images taken from this project were from my personal notebook where I planned, wrote pseudocode and made the flowcharts.

#### Arm planning

<p align="center">
  <img src="images/arm notebook ss.png" width="800">
</p>

<p align="center">
  <i>Figure 1: Arm planning notes from notebook</i>
</p>

#### SONAR planning

<p align="center">
  <img src="images/sonar notebook ss.png" width="800">
</p>

<p align="center">
  <i>Figure 2: SONAR planning notes from notebook</i>
</p>

#### Brown line following planning

<p align="center">
  <img src="images/brown line following notebook ss.png" width="800">
</p>

<p align="center">
  <i>Figure 3: Analysis of line following function</i>
</p>


#### Flowcharts
<p align="center">
  <img src="images/brown line folowing flowchart.png" width="800">
</p>

<p align="center">
  <i>Figure 4: The completed flowchart for brown line following function</i>
</p>

#### Robot in action

<p align="center">
  <img src="images/Vex robot.PNG" width="500">
</p>

<p align="center">
  <i>Figure 5: VEX robot about to pick up payload </i>
</p>

## 📚 What I Learned
- The importance of planning ahead for potential issues
- Maintaining a detailed engineering notebook of work is great practice for documenting work, ideas and troubleshooting steps
- Developing a practical understanding of proportional (P) and proportional–integral (PI) control and observing their effects on system behaviour in real time
- Translating pseudocode and flowcharts into functional, structured program code
- The use of sensor integration and the challenges of achieving reliable autonomous behaviour
