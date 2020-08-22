# Assembly Instructions

### Acquire and Print Parts

Begin by gathering all of the necessary material to build MiniQuad found in the [Master BOM](https://github.com/MiniQuad/robot/blob/master/Master%20BOM.md). Print the supplied [STL Files](https://github.com/MiniQuad/robot/tree/master/STL%20Files) in the quantities listed in the [Master BOM](https://github.com/MiniQuad/robot/blob/master/Master%20BOM.md). Note that all parts were sliced in the [PrusaSlicer](https://www.prusa3d.com/prusaslicer/) and printed on a [Prusa MK3S](https://shop.prusa3d.com/en/3d-printers/180-original-prusa-i3-mk3s-kit.html?gclid=Cj0KCQjwvvj5BRDkARIsAGD9vlIFy3uEIDK6V4373JYZdU8jZu2v4UQswNzl50jHS7kUwZr2Ial2l-0aAnDAEALw_wcB) with a 40% infill. Depending on your slicer settings and 3D Printer, material used for each part can vary. You also may need to edit the parts depending on the tolerances of your 3D printer. SOLIDWORKS files are included in the [CAD](https://github.com/MiniQuad/robot/tree/master/CAD) folder in case edits are necessary.

### Download OpenCM IDE

While the parts are printing, follow the steps to download the [OpenCM IDE](https://emanual.robotis.com/docs/en/software/opencm_ide/getting_started/) from robotis. The OpenCM IDE will be necessary to run the initial set up code as well as program MiniQuad to move. 

### Assign Motor ID's

Download and open [XL320_SetID](https://github.com/MiniQuad/robot/blob/master/Assembly%20Code/XL320_SetID.ino) in the OpenCM IDE. 

Plug 2 charged batteries into the [OpenCM9.04](http://www.robotis.us/opencm9-04-c-with-onboard-xl-type-connectors/). 

Plug one of the [XL-320](http://www.robotis.us/dynamixel-xl-320/) Motors into the OpenCM9.04 using the 3 wire cable that comes with it. 

For this step, make sure only one motor is plugged in at a time!

Plug the OpenCM9.04 into a USB Port on your computer.  

Flip the switch on the OpenCM9.04 near the batteries to the on position. If you are unsure which way is the on position, you can unplug the OpenCM9.04 from your computer. The red light will remain on when unplugged if the switch is in the correct position. 

Edit the code so that the number in the red box pictured blow is the current ID you are assigning.

Upload the code. If the motor begins to rotate back and forth, its ID has been successfully set.

Label the Motor with its ID. This will be important for future assembling as well as programming the locomotion of MiniQuad


Repeat this step for all 8 XL-320 Motors, assigning each motor with an ID of 1-8 without repeating any numbers. 

![SetID_NewID_IMG](https://user-images.githubusercontent.com/69541527/90815533-d7e38380-e2f8-11ea-86dd-e6b72a63cba3.PNG)

### Main Body Assembly

Lay the motors out in the orientation in the image below. 

![MotorLayoutIMG](https://user-images.githubusercontent.com/69541527/90822012-c5ba1300-e301-11ea-9b9b-53b30e44ea6b.PNG)

Connect Motor 1 to 2, 3 to 4, 5 to 6, and 7 to 8 with one of the supplied cables using inner terminals between each respective set of motors. Connect a second cable to the other terminals of motors 2, 3, 6, and 7. These terminals will be closest to the center of motor layout pictured above. Leave one end of the cable unnattached. This will be used to connect to the controller later.

Press a 4-40 Nut into each of the 4 holes on one of the XL320 Motor Mounts. 

![BracketNuts](https://user-images.githubusercontent.com/69541527/90821004-3e1fd480-e300-11ea-915f-31e094a18ab7.PNG)

Slide Motors 1-4 into the bracket as shown below.

![MotorIntoBracketIMG](https://user-images.githubusercontent.com/69541527/90833378-e3917300-e315-11ea-859f-60d8c88ed8b9.PNG)

Repeat the previous 2 steps with motors 5-8. Note the Orientation and order of the motors when assembling.

![MotorIntoBracket2IMG](https://user-images.githubusercontent.com/69541527/90835697-45a0a700-e31b-11ea-9495-9f1dae8f7489.PNG)

Attach both of the motor brackets to the base plate using 4-40 x .50" screws with countersunk heads (x8).

![BaseToBrackets](https://user-images.githubusercontent.com/69541527/90836069-6caba880-e31c-11ea-8b3c-84f774c28f34.PNG)

Attach the OpenCM9.04 board to the Electronics Mount using 4-40 x .50" screws. These can be countersunk, but flatheads are preferred. Note: other screw lengths over .50" may work as well.

![OpenCMMount](https://user-images.githubusercontent.com/69541527/90846716-ce790c00-e336-11ea-8aad-c52c14e4fb0f.PNG)

Attach the electronics mount to the assembly using 4-40 x .75" countersunk screws (x8) and 4-40 nuts (x8).

![EMountDOwn](https://user-images.githubusercontent.com/69541527/90917793-906cfe00-e3b1-11ea-94a5-5595f5b3b206.PNG)

After completing the above steps, the assembly should look as follows with the motor ID's corresponding to the numbers in the image below.

![BaseAssembly](https://user-images.githubusercontent.com/69541527/90847205-003ea280-e338-11ea-9c59-1575a19c8854.PNG)

### Leg Assembly

Remove the screws from the XL-320 that hold the servo horn in place (circled below)
![RemoveScrew](https://user-images.githubusercontent.com/69541527/90920506-6e29af00-e3b6-11ea-943d-a18cfbcd0f94.PNG)
