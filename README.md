# Champster

PLEASE FOLLOW THE STEPS TO HAVE A FUNCTIONING PACKET SNIFFER

Packet Sniffer for Linux
This is a packet sniffer made exclusively for Linux. The packet sniffer only works on Linux because sys is a Linux socket language only. If the packet sniffer were made for Windows it would use Winsock.

Installation:
 1. Install Linux/Ubuntu or on Vmware install Linux/Ubuntu

Vmware Ubuntu downloading instruction: 
 1. To download Vmware go to [https://www.vmware.com/products/workstation-2](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html) 
 2. player/workstation-player-evaluation.html
 3. Select Download now under "Try Workstation 17 Player for Windows" at the bottom of the page

Setting up Vmware:
 1. Download Ubuntu go to [https://ubuntu.com/download](https://ubuntu.com/download/desktop) select "Download 22.04.3" in Ubuntu 22.04.3 LTS
 2. open the Vmware's .exe file
 3. Click next until "change, repair, or remove installation"
 4. Click Change
 5. choose Add VMware Workstation console tools into the system PATH and next
 6. Once installation is done click Finish
 7. Open the VMware workstation player
 8. Choose Use VMware Workstation 17Player for free for non-commercial use
 9. click "Create a New Virtual Machine"
 10. Select "installer disc image file (iso)" and choose the downloaded Ubuntu file
 11. Enter personalize the virtual machine by entering your chosen Full name:, User name, password:, and reconfirm the password:
 12. Choose a location for the File of the Virtual machine to go
 13. Choose Maximum disk size
 14. Select split virtual disk into multiple files and click next
 15. Click Finish

**Any instruction given after this will all be within Vmware**

Setting up Ubuntu on Vmware:
 1. Select the language
 2. After selecting language select Normal installation and continue
 3. Select Erase disk and install Ubuntu
 4. Select your location
 5. Enter who you are
 6. Wait for in installation to finish
 7. Click restart computer

To run this program your Linux/Ubuntu needs to have library GTK version 2.0 and libpcap version 0.8:
 1. Open terminal in any location
 2. type "sudo apt update"
 3. type "sudo apt install libgtk2.0-dev" and type in "Y" when asked Y/n
 4. After the installation of GTK is finished
 5. type "sudo apt-get install libpcap" and type in "Y" when asked Y/n

To run this program you will also need a GUI text editor called Geany
 1. To install Geany type "sudo apt install geany" and type in "Y" when asked Y/n

From GitHub https://github.com/Nongmingren/Champster download the 3 files (main, main.c, and main.o) into your Linux/Ubuntu
 1. Organize the 3 files into a folder
 2. In the folder right-click on main.c
 3. Select "Open with Other Application"
 4. Then select Geany
 5. Click build
 6. Click Set Build Commands
 7. In the *Command* column of the *Compile* row type: gcc -Wall -c "%f"  `pkg-config --cflags --libs gtk+-2.0` -Wno-unused-function -lpcap ** Note include the ` before pkg and after 2.0
 8. In the *Command* column of the *Build* row type: gcc -Wall -o "%e" "%f"  `pkg-config --cflags --libs gtk+-2.0` -Wno-unused-function -lpcap ** Note include the ` before pkg and after 2.0

Now the setup and installation is finished

To run the program
 1. Go into the folder that the 3 files are in
 2. Right click and open terminal in the folder
 3. Type "sudo ./main"
The GUI should now pop up
Press the button to begin the packet sniffing
Try opening some websites and coming back to check the terminal
The terminal will display all the different types of packet categorized as protocol types
Also, look at the folder there will now be a log.txt file
The log.txt file will show a greater amount of information on the packets such as the packet size, the source IP, and the destination IP

