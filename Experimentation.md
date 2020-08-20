## Experiments

![The four different leg joint configurations](https://user-images.githubusercontent.com/69541527/90814555-4a536400-e2f7-11ea-8811-19adc9005cc0.jpg)

MiniQuad's stability was evaluated for both the walking and running gait by observing inertial measurement unit (IMU) readings for roll and pitch and their derivatives as the robot traversed over a straight, 1 meter long flat course. This data was recorded for four different configurations as shown in the image above for both walking and running. Two different leg trajectories, one centered and one with an offset of 17.5 mm as shown below were also considered during experimentation.
![Centered](https://user-images.githubusercontent.com/69541527/90566340-4d731680-e176-11ea-941c-d3ad530c5048.PNG)
![Offset](https://user-images.githubusercontent.com/69541527/90566381-5fed5000-e176-11ea-993e-565521c609b6.PNG)

For each experiment,five trials were conducted over eight different configuration-trajectory combinations.
The IMU readings for roll and pitch and their derivatives were stored in text files written to an SD card during the experiments. As this data was noisy and also contained readings before and after the duration of the experiment, data preprocessing was required before extracting useful information from it. The data from the text file was extracted and clipped to include the portion relevant to the experiment using MATLAB. It was desired to observe the rate at which the roll and pitch changed, and hence the derivatives were initially plotted to find that the curve was similar to an oscillation. The average amplitude of the oscillation was found for each trial and averaged over all trials on a specific joint configuration and gait to obtain the average rate at which it changed for that leg configuration and gait in order to assess the stability of the robot’s body.

### Observations
It was observed that the least rate of change in roll and pitch values for the walking gait was for configuration (b) and configuration (c) for the running gait suggesting that these could be the most stable leg configurations. However, these configurations were unable to produce gait when there leg trajectories were changed and hence it could not be concluded if these were the most stable. Configuration (d) was the only one to have produced gait for all trajectories and was also the most unstable.

