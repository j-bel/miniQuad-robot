### Assign Motor ID's

Download and open [XL320_SetID](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Code/XL320_SetID.ino) in the OpenCM IDE. 

Plug 2 charged batteries into the [OpenCM9.04](http://www.robotis.us/opencm9-04-c-with-onboard-xl-type-connectors/). 

Plug one of the [XL-320](http://www.robotis.us/dynamixel-xl-320/) Motors into the OpenCM9.04 using the 3 wire cable that comes with it. 

For this step, make sure only one motor is plugged in at a time!

Plug the OpenCM9.04 into a USB Port on your computer.  

Flip the switch on the OpenCM9.04 near the batteries to the on position. If you are unsure which way is the on position, you can unplug the OpenCM9.04 from your computer. The red light will remain on when unplugged if the switch is in the correct position. 

Edit the code so that the number in the red box pictured blow is the current ID you are assigning.

Upload the code. If the motor begins to rotate back and forth, its ID has been successfully set.

Label the Motor with its ID. This will be important for future assembling as well as programming the locomotion of MiniQuad


Repeat this step for all 8 XL-320 Motors, assigning each motor with an ID of 1-8 without repeating any numbers. 

![1SetID_NewID_IMG](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/1%20Main%20Body%20Assembly/1SetID_NewID_IMG.PNG)
