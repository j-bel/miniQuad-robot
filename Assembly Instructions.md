# Assembly Instructions

### Acquire and Print Parts

Begin by gathering all of the necessary material to build MiniQuad found in the [Master BOM](https://github.com/MiniQuad/robot/blob/master/Master%20BOM.md). Print the supplied [STL Files](https://github.com/MiniQuad/robot/tree/master/STL%20Files) in the quantities listed in the [Master BOM](https://github.com/MiniQuad/robot/blob/master/Master%20BOM.md). Note that all parts were sliced in the [PrusaSlicer](https://www.prusa3d.com/prusaslicer/) and printed on a [Prusa MK3S](https://shop.prusa3d.com/en/3d-printers/180-original-prusa-i3-mk3s-kit.html?gclid=Cj0KCQjwvvj5BRDkARIsAGD9vlIFy3uEIDK6V4373JYZdU8jZu2v4UQswNzl50jHS7kUwZr2Ial2l-0aAnDAEALw_wcB) with a 40% infill. Depending on your slicer settings and 3D Printer, material used for each part can vary. You also may need to edit the parts depending on the tolerances of your 3D printer. SOLIDWORKS files are included in the [CAD](https://github.com/MiniQuad/robot/tree/master/CAD) folder in case edits are necessary.

### Download OpenCM IDE

While the parts are printing, follow the steps to download the [OpenCM IDE](https://emanual.robotis.com/docs/en/software/opencm_ide/getting_started/) from robotis. The OpenCM IDE will be necessary to run the initial set up code as well as program MiniQuad to move. 

### Assign Motor ID's

Download and open [XL320_SetID](www.google.com) in the OpenCM IDE. Plug 2 charged batteries into the [OpenCM9.04](http://www.robotis.us/opencm9-04-c-with-onboard-xl-type-connectors/). Plug the OpenCM9.04 into a USB Port on your computer. Plug one of the [XL-320](http://www.robotis.us/dynamixel-xl-320/) Motors into the OpenCM9.04 using the 3 wire cable that comes with it. For this step, make sure only one motor is plugged in at a time! Flip the switch on the OpenCM9.04 near the batteries to the on position. If you are unsure which way is the on position, you can unplug the OpenCM9.04 from your computer. The red light will remain on when unplugged if the switch is in the correct position. Edit the code so that the number in the red box pictured blow is the current motor you are assigning. Repeat this step for all 8 XL-320 Motors, assigning each motor with an ID of 1-8 without repeating any numbers. 


![SetID_NewID_IMG](https://user-images.githubusercontent.com/69541527/90815533-d7e38380-e2f8-11ea-86dd-e6b72a63cba3.PNG)

