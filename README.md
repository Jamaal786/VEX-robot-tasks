# VEX robot tasks

## 📌 Overview
This project involved writing code for the robot to complete tasks to complete a main mission. The robot had to comply certain rules and achieve objectives at the same time to get a good overal score. My role in this project was to write code for the robot to raise and lower its arm, usage of sonar for the robot to stop a certain amount of distance away from a blockage, and aided in code tweaking of the robot following a line. I also drew up flowcharts of the necessary functions, and the main body of the code. 

## 🎯 Objectives
- Arm raised and lowered accuratey via P controller
- Robot stops certain distance away from blockage set at any distance away from payload
- Robot follows line accurately
  
## 🛠 Tools & Concepts Used
- C programming
- Concept of a PI controller

## 🔍 Methodology
#### Arm Function
For the arm function, I used the encoder from the arm and converted the encoder counts into angular degrees. This allowed an easier way to adjust the height of the arm we needed it to reach to pick up and drop off the payload. I used a P controller instead of PI as we did not need the arm to be extremely accurate and it had large operating range to carry out its job with small deviations.

#### SONAR
The SONAR function was ultised from the SONAR sensor built in the VEX robot. The distance of the blockade detected from SONAR would be relayed back. Using this value and some trial and error, I managed to get a proper distance that the VEX robot should stop away from the blockade by calling another function we wrote to ensure effecient pickup of the payload. 

#### Line Following
The line following function was mainly written by my lab partner, but after multiple failed attempts, I decided to have a look to try and adjust some of the code. In order to do that, I had to understand the whole task and plan it out on my own. In the end, I found out that the code was correct and the values we had put in for the IR sensor needed some tweaking. This particlar function was very tricky for us both as we were not strong in coding and never tackled a problem like this before. We just trial and error'ed the whole process, which ultimately ended up working in the end. However, we both knew that the function could improve and be more stable.

## 📊 Results
In the end, all of the fuctions we wrote worked. The arm and SONAR both worked quite well, although they were the simpler ones to code and tweak. The line following was particulary tricky with the amount of tweaks and adjustments we had to make. In the end, the function worked, but it was not a solid function which could work all the time. 

## 📸 Project Images
Most of the images taken from this proejct were from my personal notebook where I planned and wrote pseudocode.

#### Arm planning
![arm planning](https://github.com/Jamaal786/VEX-robot-tasks/blob/main/arm%20notebook%20ss.png)
#### SONAR planning

#### Brown line following planning

#### Flowcharts

## 📚 What I Learned

- Starting to plan on how to tackle the problem ahead is very important.
- Keeping a diary of work done is a great practice for showing work and writing down immediate ideas.
- Being able to see the effects of P and PI control in real time definitely helped with understanding it. Conceptually a difficult topic to grasp only through lectures.
- Managed to practice my ability to think in "code" and how to implement pseudocode into real code.
- I could improve by understanding how certain components in a system works ahead of class, or researching them before we begin our coding. Maybe ask more questions and definitly brush up on my coding knowledge.
