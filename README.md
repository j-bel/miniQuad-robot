# MiniQuad
### A Mini Quadrupedal Robot
CAD Files, Assembly Instruction, and Software Tutorials for a Miniature Quadrupedal Robot.  


![MiniQuad](https://user-images.githubusercontent.com/69541527/90534917-50efa900-e148-11ea-82d5-a5fc13fa7e4e.jpeg)



MiniQuad is a miniature quadruped robot capable of achieving four different leg joint configurations. It was created in order to test the impact of these different configurations on the quadruped's stability when it moves over a flat surface. The robot's body parts have been entirely 3D printed, allowing the robot to be extremely light weight. MiniQuad helps determine the viability of quadruped robots for different robotics research initiatives, as opposed to more traditional, wheeled robots, at a much lower cost.

### Assembly

Building a MiniQuad requires access to a 3D printer, a screw drive, and a pair of pliers.

The Parts List and Links to order all off the shelf parts can be found in the [Master BOM](https://github.com/MiniQuad/robot/blob/master/Master%20BOM.md). 

All of the STL files for 3D printed parts can be found in [STL Files](https://github.com/MiniQuad/robot/tree/master/STL%20Files)

Detailed Assembly Instructions can be found in [Assembly Instruction]


### Design
The main design goals were to allow multiple leg-joint configurations while minimizing the weight of the robot. In order to do this, we relocated the motors from the joints themselves. The motors on the robot are offset from the joints through the use of timing belts. The motors that control the robot’s knees are actually located at its hip joints, and the motors that control its hip joints are located near the center of the robot’s sides. Apart from using 3D printed components, mounting the actuators on the main body, helped reduce the weight of the legs. Condensing its overall size also helped minimize the robot weight while maximizing the capabilities of the actuators by enabling them to reach higher angular velocities and increasing the overall speed of the robot.

![Exploded Leg View](https://user-images.githubusercontent.com/69541527/90536027-86e15d00-e149-11ea-98bc-41dbec4e5b82.PNG)


![MiniRHex Prototype](Images/mini1.jpg)


## Experiments

![The four different leg joint configurations](https://user-images.githubusercontent.com/69541527/90563998-9cb74800-e172-11ea-97aa-886bd5febded.JPG)

MiniQuad's stability was evaluated for both the walking and running gait by observing inertial measurement unit (IMU) readings for roll and pitch and their derivatives as the robot traversed over a straight, 1 meter long flat course. This data was recorded for four different configurations for both walking and running each with 2 different leg trajectories as shown in the image. 

![Centered](https://user-images.githubusercontent.com/69541527/90566340-4d731680-e176-11ea-941c-d3ad530c5048.PNG)
![Offset](https://user-images.githubusercontent.com/69541527/90566381-5fed5000-e176-11ea-993e-565521c609b6.PNG)

For each experiment,five trials were conducted over eight different configuration-trajectory combinations.
The IMU readings for roll and pitch and their derivatives were stored in text files written to an SD card during the experiments. As this data was noisy and also contained readings before and after the duration of the experiment, data preprocessing was required before extracting useful information from it. The data from the text file was extracted and clipped to include the portion relevant to the experiment using MATLAB. It was desired to observe the rate at which the roll and pitch changed, and hence the derivatives were initially plotted to find that the curve was similar to an oscillation. The average amplitude of the oscillation was found for each trial and averaged over all trials on a specific joint configuration and gait to obtain the average rate at which it changed for that leg configuration and gait in order to assess the stability of the robot’s body.

### Observations
It was observed that the least rate of change in roll and pitch values for the walking gait was for configuration (b) and configuration (c) for the running gait suggesting that these could be the most stable leg configurations. However, these configurations were unable to produce gait when there leg trajectories were changed and hence it could not be concluded if these were the most stable. Configuration (d) was the only one to have produced gait for all trajectories and was also the most unstable.
