# CYSE-465-Autoware-Project
Below are my contributions to the CYSE 465 Autoware project: 

Autoware with Rviz:
* I gained understanding of Autoware and the perception stack of LGSVL: https://github.com/CPFL/Autoware-Manuals/blob/master/en/Autoware_UsersManual_v1.1.md
* Ran Autoware.AI 1.14.0 with SVL Simulator and Rviz (as this contributed to orignal plan to test attack on autopilot features). Commands are documented in the following link: https://www.svlsimulator.com/docs/system-under-test/autoware-instructions/

SVL with Rviz:
* Launch Autware.ai in conjunction with SVL Simulator: ./run.sh -t 1.1.4.0 and roslaunch runtime_manager runtime_manager.launch , then load each respective .launch file in Runtime Manager as stated in tutorial. For our simulation, Jack created a map on Cubetown with our adversarial object, and Kevin converted this map to cooperate with Runtime Manager as a .launch file, so This would be the only difference in loaded files. 
* I actively joined group meetings even if only viewing the VM session and offering suggestions on troubleshooting for controller: 
* Specifically, troubleshooting included fixing faulty localization which prevented Autoware.AI with Rviz to run with Mission Planning launch. Using GNSS for localization and commenting ndt_matching in my_localization.launch file did not fix issues, however. Most faults at this time were due to CPU issues. 
* CPU Issues shown below (Kevin kept in contact with GMU ORC to continuously add CPU Cores until we had 10 more added, but CPU issues persisted despite some performance increase)

![image](https://github.com/lorenzops1221/CYSE-465-Autoware-Project/blob/main/Images/rviz%20cpu.png)
* Additional troubleshooting included marking "detection" in runtime manager, as this was not stated in instructions, but performed in an instructional video: https://www.youtube.com/watch?v=cASgrZpFlEU

* LGSVL could not load map and I researched our given error. Found no similar error other than the following unresolved ticket: https://github.com/lgsvl/simulator/issues/2012 - This issue was resolved by Jack after rebooting
SVL with Apollo 5.0:
* Group eventually switched from Rviz to Apollo 5.0 after continuous issues with Rviz. Learned to run Apollo with SVL Simulator using docker/scripts/dev_into.sh, bootsraph.sh, bridge.sh: https://www.svlsimulator.com/docs/system-under-test/apollo5-0-instructions/

* Explored additional resources to get autonomous driving working: https://www.youtube.com/watch?v=781zkzN2xMg (Does not utilize perception stack), https://www.youtube.com/watch?v=cwJi1xrpj7E (Method did not work with SVL Simulator)
* Simulation set up by Jack and run by Kevin showing LiDAR not picking up cone
![image](https://github.com/lorenzops1221/CYSE-465-Autoware-Project/blob/main/Images/unnamed.png)

* Was active in group discord/discussions as shown below:


![image](https://github.com/lorenzops1221/CYSE-465-Autoware-Project/blob/main/Images/active%20member.JPG)
Additional Contributions:
* For the Autoware project writeup, I wrote the threat model portion
* For the video demonstration, I presented the threat model portion
* Threat Model details were gathered from information in the following source: https://arxiv.org/pdf/2005.03778.pdf
