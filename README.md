# CYSE-465-Autoware-Project
Below are my contributions to the CYSE 465 Autoware project: 

Autoware with Rviz:
* I gained understanding of Autoware and the perception stack of LGSVL: https://github.com/CPFL/Autoware-Manuals/blob/master/en/Autoware_UsersManual_v1.1.md
* Ran Autoware.AI 1.14.0 with SVL Simulator and Rviz (as this contributed to orignal plan to test attack on autopilot features). Commands are documented in the following link: https://www.svlsimulator.com/docs/system-under-test/autoware-instructions/

SVL with Rviz:
* I actively joined group meetings even if only viewing the VM session and offering suggestions on troubleshooting for controller: 
* Specifically, troubleshooting included fixing faulty localization which prevented Autoware.AI with Rviz to run with Mission Planning launch. Using GNSS for localization and commenting ndt_matching in my_localization.launch file did not fix issues, however. Most faults at this time were due to CPU issues. 
* Additional troubleshooting included marking "detection" in runtime manager, as this was not stated in instructions, but performed in an instructional video: https://www.youtube.com/watch?v=cASgrZpFlEU

SVL with Apollo 5.0:
* Group eventually switched from Rviz to Apollo 5.0 after continuous issues with Rviz. Learned to run Apollo with SVL Simulator using docker/scripts/dev_into.sh, bootsraph.sh, bridge.sh: https://www.svlsimulator.com/docs/system-under-test/apollo5-0-instructions/

* Explored additional resources to get autonomous driving working: https://www.youtube.com/watch?v=781zkzN2xMg (Does not utilize perception stack), https://www.youtube.com/watch?v=cwJi1xrpj7E (Method did not work with SVL Simulator)


* Was active in group discord/discussions as shown below ![image](https://github.com/lorenzops1221/CYSE-465-Autoware-Project/blob/main/Images/active%20member.JPG)
* Additionally, I wrote the threat model portion of the Autoware project writeup
