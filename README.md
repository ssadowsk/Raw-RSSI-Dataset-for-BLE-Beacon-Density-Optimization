# Raw-RSSI-Dataset-for-BLE-Beacon-Density-Optimization

This RSSI Dataset is a comprehensive set of Received Signal Strength Indicator (RSSI) readings gathered from a single environment using BLE beacons. The number of beacons was scaled from 3 to 8 performing the same analysis to determine the optimal number that produces results with the lowest error.
 
For the experimentation, the transmitters used consisted of Gimbal Series 10 Beacons and a Raspberry Pi 3 Model B being used a the receiver.
 
   <p align="center">
Gimbal Series 10 Beacon   
  </p>

<p align="center">
 
 <img src="https://github.com/ssadowsk/Raw-RSSI-Dataset-for-BLE-Beacon-Density-Optimization/blob/master/Images/iBeacon_Gimbal_Series10.png">
 </p>
 
# Experiment
A set of tests was conducted to determine the accuracy between multiple types of system designs including: Trilateration, and Nonliner Least Squares while using a moving average and Kalman filter. For the experiments all tests were done on tables which allowed tests to be simulated at a height where a user would be carrying a device in their pocket. Devices were also kept in the same orientation throughout all the tests in order to reduce the amount of error that would occur in the measuring of RSSI values. 
 
 ## Environment
Experiments were performed in a single environment.

The testing environment used was a 10.8 x 7.3 m computer lab. This lab was a large area with a typical amount of noise occuring due to the WiFi and BLE transmitting that were in the area. The large space also allowed for signals to experience obstructions, reflections, and interference. Transmitters were placed inorder for Line-of-Sight (LoS) to be available between the transmitters to the receiver.
 
 ## Topology
 In the testing environemnt, fingerprints were gathered to be used in the creation of a database, while tests points were selected to be used against the database for the comparison. In the figures the black dots represent the location of the transmitters and the red dots represent the locations where fingerprints and tests points were gathered where appropiate. A general overview of the experimental topologies performed can be seen here:


 <p align="center">
Experiment Layout
  </p>

<p align="center">
 
 <img src="https://github.com/ssadowsk/Raw-RSSI-Dataset-for-BLE-Beacon-Density-Optimization/blob/master/Images/layout.png">
 </p>

 # Related Publications
 
 To be added...
 
 # Dataset
The RSSI dataset is seperated based on the number of transmitters and the position of the receiver. For specific locations, the (x,y) coordinates can be seen in Test.xlsx.

For the files in the Database and Tests folders there are approximatly 300 reading. Readings appear in the format "*Number* = *Value* *Timestamp*" where:

*Number* corresponds to the transmitter that signal was sent from, represented by '1', '2', ... , upto '8'.

*Value* is the RSSI reading.

*Timestamp* is a timestamp of when the reading was taken.
