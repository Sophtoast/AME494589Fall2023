Julien Purvis, Sophie Armstrong
Tejaswi Linge Gowda
Programming for IoT
01 December, 2023
Customizable Health Analytics
A common issue with modern health-tracking technologies like the Apple Watch and Fitbit is the need for more open-source and customizable options. This project aims to create a health analytics wearable that could be openly modified and modularly added to fit an individual's needs. For example: if an individual is particularly concerned about the quality of their sleep a watch that prioritizes passive analytics and longer battery life would be more useful than one that focuses on intermittent monitoring and athletic diagnostics. Because of this, the most useful watch would be one that can evolve with the user's needs.
Initial Ambitions.
The initial goals of this project were to combine sensors reading accelerometer, gyroscopic, magnetometric, and Holter monitor data to get comprehensive diagnostics about a user's health and health-related behaviors. The root of the project lies in monitoring the steps and physical activity of the user and providing them with useful statistics that could tell them about their habits and encourage them to continue their exercise. The goal was to send the data as a computed orientation and a live heart rate over HTTP to a server that would run analytics and display the data to the user.


Initial design diagram of the pedometer system.
  







What we achieved.
We used a Lilygo MPU9250 for our orientation data and core computations. It successfully computes orientation using a Madgwick filter and sends it to a server. The device can connect to wifi and communicate reliably. On the server side, the server can reliably receive and display the orientation data. An implementation of the data analysis for step recognition and graphing of the steps has been added however it is non-functional at this time.
Transport and display of orientation data on the server.
  



The design gap.
        While some of the bones of the project are missing it was somewhat overscoped and the learning curve was too steep for some of the functionality stated in the initial goals. There is no heart rate monitor and no hardware was identified for it, and the data analysis portion has been rather unsuccessful. For this to be a usable product, we believe there would be significant research and time needed to develop and train accurate data analysis functions and a more comprehensive system of interfaces for the user to interact with.
Reflection -Sophie Armstrong: 
        I started this class being very unfamiliar with working with servers and new to HTML. Since then I have had a greater understanding of blue tooth devices and how data collection works across the internet. I have a greater appreciation for what goes into web development as well as a greater grasp on the resources to work in that field. I no longer have as much hesitation when faced with IoT tasks as I once did. I understand how to check if I run into issues and troubleshoot.