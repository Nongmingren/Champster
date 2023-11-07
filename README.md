# Champster

PLEASE FOLLOW THE STEPS TO HAVE A FUNCTIONING PACKET SNIFFER

Packet Sniffer for Linux
This is a packet sniffer made exclusively for Linux. The packet sniffer only works on Linux because sys is a Linux socket language only. If the packet sniffer were made for Windows it would use Winsock.

Installation:
 1. Install Linux/Ubuntu or on Vmware install Linux/Ubuntu

Vmware Ubuntu downloading instruction [If using Vmware (if not skip to line ...)]: 
 1. To download Vmware go to [https://www.vmware.com/products/workstation-2](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html) 
 2. player/workstation-player-evaluation.html
 3. Select Download now under "Try Workstation 17 Player for Windows" at the bottom of the page

Setting up Vmware:
 1. Download Ubuntu go to [https://ubuntu.com/download](https://ubuntu.com/download/desktop) select "Download 22.04.3" in Ubuntu 22.04.3 LTS
 2. open the Vmware's .exe file
 3. click "Create a New Virtual Machine"
 4. Select "installer disc image file (iso)" and choose the downloaded Ubuntu file
 5. Enter personalize the virtual machine by entering your chosen Full name:, User name, password:, and reconfirm the password:

**Any instruction given after this will all be within Vmware**

To run this program your Linux/Ubuntu needs to have library GTK version 2.0 and libpcap version 0.8:
 1. Open terminal in any location
 2. type "sudo apt update"
 3. type "sudo apt install libgtk2.0-dev" and type in "Y" when asked Y/n
 4. After the installation of GTK is finished
 5. type "sudo apt-get install libpcap" and type in "Y" when asked Y/n

To run this program you will also need a GUI text editor called Geany
 1. To install Geany type "sudo apt install geany" and type in "Y" when asked Y/n

From GitHub download the folder into your Linux/Ubuntu


The benefits of packet sniffer:
  1. When encountering network problems you can use the packet sniffer to identify the root problem.
