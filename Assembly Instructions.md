# Assembly Instructions

### Acquire and Print Parts

Begin by gathering all of the necessary material to build MiniQuad found in the [Master BOM](https://github.com/MiniQuad/robot/blob/master/Master%20BOM.md). Print the supplied [STL Files](https://github.com/MiniQuad/robot/tree/master/STL%20Files) in the quantities listed in the [Master BOM](https://github.com/MiniQuad/robot/blob/master/Master%20BOM.md). Note that all parts were sliced in the [PrusaSlicer](https://www.prusa3d.com/prusaslicer/) and printed on a [Prusa MK3S](https://shop.prusa3d.com/en/3d-printers/180-original-prusa-i3-mk3s-kit.html?gclid=Cj0KCQjwvvj5BRDkARIsAGD9vlIFy3uEIDK6V4373JYZdU8jZu2v4UQswNzl50jHS7kUwZr2Ial2l-0aAnDAEALw_wcB) with a 40% infill. Depending on your slicer settings and 3D Printer, material used for each part can vary. You also may need to edit the parts depending on the tolerances of your 3D printer. SOLIDWORKS files are included in the [CAD](https://github.com/MiniQuad/robot/tree/master/CAD) folder in case edits are necessary.

### Download OpenCM IDE

While the parts are printing, follow the steps to download the [OpenCM IDE](https://emanual.robotis.com/docs/en/software/opencm_ide/getting_started/) from robotis. The OpenCM IDE will be necessary to run the initial set up code as well as program MiniQuad to move. 

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

### Main Body Assembly

Lay the motors out in the orientation in the image below. 

![2MotorLayoutIMG](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/1%20Main%20Body%20Assembly/2MotorLayoutIMG.PNG)

Connect Motor 1 to 2, 3 to 4, 5 to 6, and 7 to 8 with one of the supplied cables using inner terminals between each respective set of motors. Connect a second cable to the other terminals of motors 2, 3, 6, and 7. These terminals will be closest to the center of motor layout pictured above. Leave one end of the cable unnattached. This will be used to connect to the controller later.

Press a 4-40 Nut into each of the 4 holes on one of the XL320 Motor Mounts. 

![3BracketNuts](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/1%20Main%20Body%20Assembly/3BracketNuts.PNG)

Slide Motors 1-4 into the bracket as shown below.

![4MotorIntoBracketIMG](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/1%20Main%20Body%20Assembly/4MotorIntoBracketIMG.PNG)

Repeat the previous 2 steps with motors 5-8. Note the Orientation and order of the motors when assembling.

![5MotorIntoBracket2IMG](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/1%20Main%20Body%20Assembly/5MotorIntoBracket2IMG.PNG)

Attach both of the motor brackets to the base plate using 4-40 x .50" screws with countersunk heads (x8).

![6BaseToBrackets](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/1%20Main%20Body%20Assembly/6BaseToBrackets.PNG)

Attach the OpenCM9.04 board to the Electronics Mount using 4-40 x .50" screws. These can be countersunk, but flatheads are preferred. Note: other screw lengths over .50" may work as well.

![7OpenCMMount](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/1%20Main%20Body%20Assembly/7OpenCMMount.PNG)

Attach the electronics mount to the assembly using 4-40 x .75" countersunk screws (x8) and 4-40 nuts (x8).

![8EMountDOwn](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/1%20Main%20Body%20Assembly/8EMountAttach.PNG)

After completing the above steps, the assembly should look as follows with the motor ID's corresponding to the numbers in the image below.

![9BaseAssembly](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/1%20Main%20Body%20Assembly/9BaseAssembly.PNG)

### Leg Assembly

Remove the screws from the XL-320 that hold the servo horn in place (circled below)
![1RemoveScrew](https://user-images.githubusercontent.com/69541527/90920506-6e29af00-e3b6-11ea-943d-a18cfbcd0f94.PNG)


![1_2MotorZero](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/2%20Leg%20Assembly/1_2MotorZero.PNG)

![2MotorHubNuts](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/2%20Leg%20Assembly/2MotorHubNuts.PNG)

![3AttachMotorHub](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/2%20Leg%20Assembly/3AttachMotorHub.PNG)

![4MotorHubConnectorLockNut](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/2%20Leg%20Assembly/4MotorHubConnectorLockNut.PNG)

![5MotorHubConnScrews](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/2%20Leg%20Assembly/5MotorHubConnScrews.PNG)

![6PulleyBrace](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/2%20Leg%20Assembly/6PulleyBrace.PNG)

![7SetZeroCode](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/2%20Leg%20Assembly/7SetZeroCode.PNG)

![8ThighAndTimingBelt](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/2%20Leg%20Assembly/8ThighAndTimingBelt.PNG)

![9KneePulley](https://github.com/MiniQuad/robot/blob/master/Assembly%20Files/Assembly%20Images/2%20Leg%20Assembly/9KneePulley.PNG)
