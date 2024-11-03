# Raspberry Pi 0 2W - pwnagotchi 

  > [!WARNING]
  > I do not encourage or support the unauthorised use of pwnagotchi for malicious activities. The information and details I provide are for educational purposes only. 

## Objective
Build and set up my own pwnagotchi to scan for my networks and test the strength of my passwords using hashcat.

## Introduction
With an introduction into cybersecurity I came across some videos of pentration testing of a device called a pwnagotchi, not to go into too much detail as the official website linked [here](https://pwnagotchi.ai/usage/#anatomy-of-a-pwnagotchi-face) has so much more information I am still working and learning through. Briefly the software pwnagotchi uses the built in wifi in the Raspberrypi 0 to scan for networks and attempts to capture handshakes with other networks and store the information as a pcap for review on it's storage. The displays shows an image that ressembles a tomigotchi displaying various faces to indicate it's mood and personality again more information can be found [here] (https://pwnagotchi.ai/intro/#the-faces) and some text on what it's doing.  

## Tools Used: 
Hardware build: 
 - [RaspberryPi 0 2W](https://www.aliexpress.com/item/1005007480776599.html?spm=a2g0o.productlist.main.3.65eccVmmcVmmyz&algo_pvid=14c9d7c4-709a-43c6-b532-dbc1c1a2eae3&utparam-url=scene%3Asearch%7Cquery_from%3A)
 - [Waveshark 2.13 inch e-Paper HAT](https://www.aliexpress.com/item/33005909532.html?spm=a2g0o.store_pc_home.promoteWysiwyg_494620227.33005909532)
 - 8GB micro SD card
 - External powerbank
 - USB cable with micro usb
   
Software: 
 - [jayofenloy Repo](https://github.com/jayofelony/pwnagotchi)
 - [balenaEtcher](https://etcher.balena.io/) 
 - [WinSCP](https://winscp.net/eng/download.php)
 - [hashcat](https://hashcat.net/hashcat/)
 - [hashcat coverter](https://hashcat.net/cap2hashcat/)

Other Resources:
- Wordlist text files such as: Rockyou.txt 

# Installation:
  1. With the hardware it's an easy assemble, raspberrypi has the gpio with headers installed so connecting the e-ink display is as simple as lining up the pins and pushing them in.
     
  2. The software build took some time, initially I had a SD card ordered with AliExpress but due to the SD card build it wasn't reliable which cost me a good few hours wondering why the raspberry wasn't working. Issues such as:
     - Failed writes
     - Board not responding
     - Questioning methods
     - Formatting investigations
       
  > [!IMPORTANT]
  > Long story short, INVEST IN A GOOD QUALITY SD CARD AND DON'T CHEAP OUT
     
  3. Following this comprehensive [installation and configurations guide](https://github.com/jayofelony/pwnagotchi/wiki) I was able to setup and start my very own pwnagotchi.

# Operation: WIP
  1. Operating the pwnagotchi is as simple as plugging in power to the power port and taking a walk around to scan your network/s.
  2. Once captured a few we can use WinSCP to transfer files over to our laptop/computer to view the files, they will be in pcap format so you can use Wireshark to view what exactly has been captured but in order to work with hash cat we can upload them using hashcat coverter to change them to h2000 files. 
  3. Once converted we can move the file into our hashcat directory where our hashcat.exe file is.
  4. Opening command prompt and change our location we can list out what is available to us in this directory.
  5. The wordlist mentioned in the other resources should be located here for convience when using hashcat.
       
# Skills Learned: 
In this project I learned how to: 
- Flash images using balenaEtcher
- Set up a static IP address for my pwnagotchi
- Use Powershell to SSH into my pwnagotchi to configure name and details of device
- Use WinSCP to transfer files to laptop/PC
- Use command line prompt with hashcat
  
      
# Conclusion: 
WIP

# References: 
  
      
