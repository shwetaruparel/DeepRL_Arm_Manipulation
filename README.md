
# Deep RL Arm Manipulation

Refer the documentation about the project and information about HyperParameters and Result here - 
https://github.com/shwetaruparel/DeepRL_Arm_Manipulation/blob/master/DeepRLArm.pdf

***Refer to the project folder and find two files 
ArmPlugin_task1.cpp
ArmPlugin_task2.cpp

***Take each file one by one and copy the content to ArnPlugin.cpp in gazebo folder, build the directory and see the results for task1 and task2 respectively.

This project is based on the Nvidia open source project "jetson-reinforcement" developed by [Dustin Franklin](https://github.com/dusty-nv). The goal of the project is to create a DQN agent and define reward functions to teach a robotic arm to carry out two primary objectives:

1. Have any part of the robot arm touch the object of interest, with at least a 90% accuracy.
2. Have only the gripper base of the robot arm touch the object, with at least a 80% accuracy.

## Building from Source (Nvidia Jetson TX2) and Project Environment.

The project folder in Udacity provided Workspace is loaded in RoboND-DeepRL-Project folder, and can be found in the /home/workspace directory.

To launch the project for the first time, run the following in the terminal of the desktop gui:

$ cd /home/workspace/RoboND-DeepRL-Project/build/x86_64/bin
$ ./gazebo-arm.sh

Each task needed is completed by modifying the ArmPlugin.cpp located in gazebo folder
Build the folder and run the simulator by running following commands
$ cd build
$ make
$ cd x86_64/bin
$ ./gazebo-arm.sh

## Testing the API
Test the API for the following
1. Successfully creating the DQN Agent
2. Subscribe to camera node and collision topics
3. Define the velocity or position based control of the arm joints.
4. Assign reward for the robot gripper hitting the ground
5.Issue an interim reward based on the distance to the goal.
6. Issue a reward based on collision between the arm and the object.
7. Tune the HyperParameters and achieve an accuracy of 90 percent for the previous task.
8. Issue a Reward based on collision between the arms gripper base and the object.
9. Tune the HyperParameters and achieve an accuracy of at least 80 percent for the previous task.

