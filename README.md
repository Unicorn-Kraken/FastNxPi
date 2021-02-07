# Install Nx Witness on Raspberry Pi 4B

The process and download should take about 1 hour on a 12Mbps internet connection

**Apparatus**

- Raspberry Pi (rpi) 4B - 2/4/8GB
- SD Card for rpi
- USB C Cable for rpi
- USB Power Supply – with 5.1V / 3.0A DC output for rpi
- Device running Windows, macOS or Ubuntu with an SD card Reader
- Router/switch
- Internet Connection to download rpi image and Nx Software

**Method**

Download the Raspberry Pi Imager for you OS from one of the links below

- [https://downloads.raspberrypi.org/imager/imager\_1.4.exe](https://downloads.raspberrypi.org/imager/imager_1.4.exe)
- [https://downloads.raspberrypi.org/imager/imager\_1.4.dmg](https://downloads.raspberrypi.org/imager/imager_1.4.dmg)
- [https://downloads.raspberrypi.org/imager/imager\_1.4\_amd64.deb](https://downloads.raspberrypi.org/imager/imager_1.4_amd64.deb)

Install the Raspberry Pi Imager Software.

Insert your SD Card into your computer.

Open the Raspberry Pi Imager software and click Raspberry Pi OS (other), then select Raspberrry Pi OS Lite (32-Bit) . Select the SD card then click write. The image will be downloaded in the background and it will be written to your SD card. This time will vary based on your internet connection speed.

Since we&#39;re not using a monitor, we&#39;ll need to access the Raspberry via SSH to install the Nx Software. Go to the SD card root directory and create a new file called ssh. Doing this will enable SSH on the rpi.

Insert your newly imaged SD card into your Raspberry Pi, connect to you router and power it on.

For the next step, if you&#39;re using Windows, you&#39;re going to need to download and insall Putty [https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

Now we need to find the IP address of your Raspberry Pi. You will need to wait five minutes for the device to boot. Then, i **n Windows, Ubuntu or macOS, open the command prompt/terminal then type** arp -a - your rpi will be the device that has the physical address starting with &quot;b8-27-eb&quot; or &quot;dc:a6:32&quot;

Connect via SSH using the IP address of your rpi. The username is pi and password is raspberry.

Download the Nx Software using following command

```wget https://updates.networkoptix.com/default/31398/arm/nxwitness-server-4.1.0.31398-linux_arm32.deb```

Install Using this command

```sudo dpkg -i ./nxwitness-server-4.1.0.31398-linux\_arm32.deb```

Follow the prompts to install the Nx Software.

Install the Nx Client Software on your Windows/Ubuntu/macOS device to complete the Setup and add cameras.

Clients can be downloaded [here](https://nxvms.com/download)

```

```
