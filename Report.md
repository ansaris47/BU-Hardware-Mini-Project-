Sohaib Ansari and Julian Leguizamon
EC463
Hardware Mini Project 



Set Up

For setup, it was required for us to obtain an SD card and any accompanying adapters if needed. Initially, there was some confusion on our part as we had 
purchased a regular SD card, unbeknownst to us that they are only compatible with micro SD cards. Installing the OS was fairly simple however, we did run into 
trouble due to just being unfamiliar to how our Raspberry Pi’s operate. Understanding that the OS is installed through the SD card which is then inserted into 
the Pi and that the lab monitors are utilized as a display for the Pi helped smooth out the process. Initially, we kept brute forcing the install file into the 
SD card, not realizing we must open the file package on our personal computer to then have the OS written into the micro SD. Setting up the display and getting 
the Pi powered up was rather easy; There were no complications with the Pi and mouse/keyboard user input. Ultimately, the most complicated task for the project 
was getting an internet connection established to our Pi. We did not utilize the SSH connection because we did not have an ethernet cable nor did our Macs have 
ethernet ports. To avoid the hassle of purchasing another adapter, we decided to go the route of using a wifi hotspot for the entirety of this assignment. We 
spent several hours trying to troubleshoot the BU Wifi, however, it didn’t seem like a possibility due its security parameters.  


Running Code

When running the code we encountered very little difficulties. We first ran the commands on the Raspberry Pi to update python by using the terminal and besides 
some grammar errors had no trouble getting python up and running on the Pi. After that we ran the ble_scan.py script and were able to successfully read the 
bluetooth devices in the room with no issues. We then moved on to the wifi_scan.py. We ran it but we didn’t realize that we had to change the parameter ~/data to 
specify the directory of the JSON file, so as a result we had to run it again and specify a new directory. Additionally, the default 100 cycles only ran for 
around 8 minutes so to get the 15+ minutes of data we changed it to 220 cycles. 


Plots/Data

Figure 1: Data when the Raspberry Pi was placed in the middle of the room:
https://github.com/ansaris47/BU-Hardware-Mini-Project-/blob/beaf2154dba408c3e115497a3e69143349221d5e/test1middle.png



Figure 2: Data when the Raspberry Pi was placed next to the window: 
https://github.com/ansaris47/BU-Hardware-Mini-Project-/blob/02b55a3c704c85e03e7e9b202a5d1455f487fcd8/test2window.png



We ran the wifi_scan.py to create the JSON file but since we only specified 100 cycles it only ran for around 8 minutes and didn’t collect much data. As a 
result, we increased the cycles to 220 and moved our Raspberry Pi closer to the window so that we can pick up data from passing cars. This yielded much better 
results as we were able to collect data for over 15 minutes and get higher quality data.
