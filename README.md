# kerberosPi
This shows the user how to successfully setup the Raspberry Pi and Kerberos to work in tandem in order to identify RF signals emitted by a variety of devices. 
All links to orginal posts and hardware used with be added at the end. 

SBC: 
Download this image and unzip the package to a local place - https://drive.google.com/open?id=1DhCLYv99QHwpJRM2gvG6UtrIM1RO8_Ua
Above should be the latest version, but if not then follow this link to see any other versions - https://www.rtl-sdr.com/ksdr/ 

Disk Burning Software: 
Below are two different disk burning software that can be used to download the software to a micro SD card (minimum of 16 gig) that will be used in the raspberry pi. 
I personally used the second link (etcher) and had no problems with it. 
https://sourceforge.net/projects/win32diskimager/
https://www.balena.io/etcher/

Boot: 
Once the program is burned to the micro SD card insert it into the Pi. 
Connect the micro USB cord to the correct Kerberos port, which should be the far left one from the USB port. Connect the USb end to the raspberry pi. 
If under volted, connect an additional micro USB cable to the Kerberos left over port and then connect the other end to a power source. 
Once all of that is connect, connect the power cable to the raspberry pi and let it boot. 

Onboard: 
When the pi boots the kerberosSDR application will pop up, it may take a minute. 
You can connect to the kerberos from any other device by doing the following. 
First: Connect to the wifi emitted from the pi named: KererosPi and the password should be KerberosPi 
Second: you can access the compass from the following link. 192.168.4.1:8081 
You can focus the identification from the following link: 192.168.4.1:8080 
Third: Identify which signal you would like to track and customize the program. 

Below are the frequency calculatiosn that I have done. Whether they are right will be updated soon. (the excel file will be added to the repsitory.) 
The total distance will be the distance that the antennas will have to be placed apart. 
Type 	Frequency 	Wavelength (cm)	Wave Velocity (constant m/s) 	Spacing Factor (constant)	Total Distance (cm)
Security Camera 	2.4 GHz	12.4913524166667	299792458	0.3	3.747405725
Bluetooth	2.45 GHz	12.2364268571429	299792458	0.3	3.67092805714
4G/ LTE	700 → 2600 MHz	42.827494 → 11.530479153846153	299792458	0.3	12.8482482 → 3.45914374615
3G	1900 MHz	15.7785504210526	299792458	0.3	4.73356512632
Laptop	2.4 → 5.0 GHz	12.4913524166667 → 5.99584916	299792458	0.3	3.747405725 → 1.798754748

Links: 
Orginal kerberos set up guide: https://www.rtl-sdr.com/ksdr/
Supporting Video: https://www.youtube.com/watch?v=n5aWrz-42qc
Frequency Calculator: http://www.procato.com/calculator-wavelength-frequency/
Compass: http://192.168.4.1:8081/
Specification: http://192.168.4.1:8080/init
