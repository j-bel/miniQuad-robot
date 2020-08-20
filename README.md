# MiniQuad
### A Mini Quadrupedal Robot
CAD Files, Assembly Instruction, and Software Tutorials for a Miniature Quadrupedal Robot.  


![MiniQuad](https://user-images.githubusercontent.com/69541527/90534917-50efa900-e148-11ea-82d5-a5fc13fa7e4e.jpeg)



MiniQuad is a miniature quadruped robot capable of achieving four different leg joint configurations. It was created in order to test the impact of these different configurations on the quadruped's stability when it moves over a flat surface. The robot's body parts have been entirely 3D printed, allowing the robot to be extremely light weight. MiniQuad helps determine the viability of quadruped robots for different robotics research initiatives, as opposed to more traditional, wheeled robots, at a much lower cost.

### Assembly

Building a MiniQuad requires access to a 3D printer, a phillips head screw driver, and a pair of pliers.

The Parts List and Links to order all off the shelf parts can be found in the [Master BOM](https://github.com/MiniQuad/robot/blob/master/Master%20BOM.md). 

All of the STL files for 3D printed parts can be found in [STL Files](https://github.com/MiniQuad/robot/tree/master/STL%20Files)

Detailed Assembly Instructions can be found in [Assembly Instructions](https://github.com/MiniQuad/robot/blob/master/Assembly%20Instructions.md)

### Design
The main design goals were to allow multiple leg-joint configurations while minimizing the weight of the robot. In order to do this, we relocated the motors from the joints themselves. The motors on the robot are offset from the joints through the use of timing belts. The motors that control the robot’s knees are actually located at its hip joints, and the motors that control its hip joints are located near the center of the robot’s sides. Apart from using 3D printed components, mounting the actuators on the main body, helped reduce the weight of the legs. Condensing its overall size also helped minimize the robot weight while maximizing the capabilities of the actuators by enabling them to reach higher angular velocities and increasing the overall speed of the robot.

[Exploded Leg View](https://user-images.githubusercontent.com/69541527/90536027-86e15d00-e149-11ea-98bc-41dbec4e5b82.PNG)

## Experiments
Details about the experiments conducted can be found in [Experimentation](Experimentation.md)
