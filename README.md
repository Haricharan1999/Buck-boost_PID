### PID control of buck boost converter Using MATLAB simulink
___

## Introduction
___

The output voltage in a power electronics converter can vary with change in input voltage or change in the load or changes in duty cycle of the switching device. 
To obtain a constant output voltage, need of a controller is of outmost important. In many practical areas like pv solar plant input voltage varies significantly, this in return will also make the output dc voltage, which is very much undesirable.
## Software Required
Install MATLAB software from here https://in.mathworks.com/products/matlab.html
Also make sure to include Simscape Electricals toolbox while installing Matlab software.

## Design of PID and Instruction
___

Vo = (D*Vin)/(1-D);

where Vo=Output voltage, D=duty cycle, Vin=Input Voltage.

In a buck boost conveter we can change the ouput voltage by varying the duty cycle of the converter.
This concept is employed in the PID controller design of the buck boost converter.
Here in this project I have assumed the reference voltage to be -13v.
You can change the reference voltage by double clicking on the V_ref block of the Buck_boost_PID.slx file provided in the Simulink Files.
A buck boost converter without PID controller tunning is provided in the Simulink Files folder with name Buck_Boost_converter.slx.
The parameter values used in the project are provided in the Sytem Parameter folder.
To tune the PID controller, double click the PID block of the Buck_boost_PID.slx file.
Click the tune button inside the PID dialogue box.
## Reference 
___
https://www.saranathan.ac.in/emagazine/eee/sj/vol1_1/sjeee9.pdf
https://in.mathworks.com/help/slcontrol/gs/automated-tuning-of-simulink-pid-controller-block.html
