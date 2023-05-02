Download Link: https://assignmentchef.com/product/solved-cpe470-670-project-1-mobile-robot-localization-using-kalman-filter
<br>
Given the data collected by the real/physical Novatel DGPS, Mircostrain IMU 3DM-GX2, and Seekur robot encoders.

<ol>

 <li>Design the Kalman filter to fuse GPS, IMU and Wheel Encoder data to output a smooth and more accurate pose (position and orientation) of the robot</li>

 <li>Write Matlab or C/Cpp code (or other languages you prefer) to implement the Kalman filter (The code must be written by you. Do NOT use or copy code from online sources. Plagiarism will be 0 grade penalty.)</li>

 <li>Write a report of the project

  <ol>

   <li>Explain why the KF outperforms the individual sensor (GPS, IMU and Encoder)</li>

   <li>Report the results to prove the concept. Give text explanation for your obtained results.</li>

   <li>Change the covariance of the sensor data (GPS) and check the output of the KF, then plot and explain your observation in the report.</li>

  </ol></li>

</ol>

+ add noise to GPS covariance to all the data set

+ add noise to certain periods of GPS covariance data

<ol>

 <li>Change the covariance of the sensor data (IMU) and check the output of the KF, then plot and explain your observation in the report.</li>

</ol>

+ add noise to IMU covariance to the entire data set

+ add noise to certain periods of IMU covariance data

<ol>

 <li>Add noise to GPS position with changed covariance (added in item (c)) to see how the KF work. Plot and explain the obtained results.</li>

</ol>

+ add noise to GPS position to the entire data set

+ add noise to certain periods of GPS position data

<ol>

 <li>Put all the source code/software in the Appendix with instruction of running the code</li>

</ol>

<ol start="4">

 <li><strong>Project Deadline: March 1st, 2022. </strong></li>

</ol>

<strong>Submit the project report into Canvas. </strong>

(Note: need to calibrate IMU data to match with Odometry data for orientation fusion.)

Appendix:

Date file name: EKF_DATA_circle.txt




Data header:

%time,field.O_x,field.O_y,field.O_t,field.I_t,field.Co_I_t,field.G_x,field.G_y,field.Co_gps_x,field.Co_gps_y

Where:

<em>%time</em> is time index

<strong>Odometry or Encoder data from Seekur Mobile robot</strong>

<em>field.O_x</em> is Odometry data in x direction/coordinate of the robot

<em>field.O_y</em> is Odometry data in y direction/coordinate of the robot

<em>field.O_t</em> is Odometry data of the orientation or heading of the robot

(For the covariance of the Odometry data you can give a specific number, for example: 0.001.)

<strong> </strong>

<strong>Data from Microstrain IMU attached on the robot</strong>

<em>field.I_t</em> is IMU data of the orientation or heading of the robot

<em>field.Co_I_t </em> is the IMU data of the Covariance of the orientation of the robot







<strong>Novatel DGPS  data attached on the robot</strong>

<em>field.G_x</em> is GPS data in x direction/coordinate of the robot

<em>field.G_y</em> is GPS data in y direction/coordinate of the robot

<em>field.Co_gps_x</em> is GPS data of the Covariance in x direction of the robot

<em>field.Co_gps_y</em> is GPS data of the Covariance in y direction of the robot





