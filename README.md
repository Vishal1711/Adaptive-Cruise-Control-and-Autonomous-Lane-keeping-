# Adaptive-Cruise-Control-and-Autonomous-Lane-keeping
Academic Project at Clemson University - International Centre for Automotive Research 
### -----Can't share code here due to academic restrictions-----


## Problem Statement:

### Design and implemention of an embedded controller based on ultrasonic sensors to run down hill as fast as possible.

Achieved the following functions:

1. Adaptive Cruise Control
   - Keep the RC vehicle 30 cm away from obstacles ahead.
   - If obstacle ahead is stationary, vehicle should stop at 30 cm from obstacle.
 
2. Autonomous Lane Keeping
   - Keep the vehicle along the center of a defined lane.

## Technical Approach:

#### 1. Reinforcement Learning-
The objective of RL is to maximize the reward of an agent by taking a series of actions in response to a dynamic environment. Q-learning algorithm is taken into account to solve this problem. Q-learning is a values-based learning algorithm. Value based algorithms updates the value function based on following Bellman equation.

![image](https://user-images.githubusercontent.com/79803663/151205157-33683ad5-97f9-4ad9-8be8-cee99d868ce3.png)

### 2. PID Controller-
PID controller is non-model based controller. PID is a proportional, integrative and derivative controller. In PID there is no need to model the system relationship between input and output. PID compute the system input based on error directly. Used for throttle control and steering control.

![image](https://user-images.githubusercontent.com/79803663/151205389-ecdaa009-00f7-4e87-960d-e1fd305b47ef.png)

### **Not sucessfull in implementation with RL method. Solved this with PID Controller.**

## Hardware Implementation:

1. Arduino Uno Rev3

![image](https://user-images.githubusercontent.com/79803663/151206070-b12a35fd-e904-4659-b269-57ca05372afe.png)

2. Ultrasonic Sensor HC-SR04 

![image](https://user-images.githubusercontent.com/79803663/151206123-4c68926d-6f84-4e96-90f7-b11b5fabf3a1.png)

3. Ultrasonic sensor (1) for detecting obstacle ahead and other two sensor for lane keeping

![image](https://user-images.githubusercontent.com/79803663/151206254-e97cee80-64a4-4440-a9e7-ac16837bab26.png)

4. Electronic Speed Controller and servo motor to steer the vehicle.

![image](https://user-images.githubusercontent.com/79803663/151206664-fdca3663-0055-4dc5-94fa-aa296da4ca61.png)


## Vehicle Testing on Track:




 



https://user-images.githubusercontent.com/79803663/151207114-b9c86c7f-b583-4e11-be38-d84be69769d5.mp4



