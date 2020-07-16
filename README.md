# macOS.Catalina.Hackintosh.on.Dell.Lattitude.5590
MacOS Catalina Hackintosh Built on Dell Lattitude 5590 Model 

My Laptop Configuration

* SSD: SK hynix SC311 SATA 256GB
* Processor: 2.6 GHz Dual-Core Intel Core i3
* Graphics: Intel HD Graphics CFL CRB 1536 MB
    Display:
    Resolution:	1920x1080 (1080p FHD - Full High Definition)
    UI Looks like:	1920 x 1080 @ 60 Hz
    VRAM (Dynamic, Max):	1536 MB
* RAM : 20 GB (4GB soldered onboard + 16 GB)


What is working ?

+ Display with FHD resolution: Onboard graphics UHD630
+ Bluetooth
+ Sound on earphones only and on bluetooth speakers 
    Note: I am using one Plus bullet earphones on USB Type C port which is working for me. Not tested on 3.5 mm jack. Probably it will not work.
+ Trackpad but without Apple trackpad gestures
+ Battery indicator 
    Note: As 10th Gen Intel processors are new to Hackintosh, respective patches are work in progress. 
    In my case battery of the laptop was draining fast due to issue that processor was always running into Turbo Boost mode. 
    I disabled the same from Bios and since then my laptop give easily 4-4.5 hours of battery life after tunning the running services.
+ Brightness Controller
+ USB2/3 Ports, TypeC ports, SD-Card Reader Port
+ Screen off after inactivity
+ Audio on internal laptop speaker

What is not working ?

- Wifi 
  Note: (Workaround) : Bought a new USB Wifi dongle and installed the latest version of software from https://github.com/chris1111/Wireless-USB-Adapter,
  I am using D-Link DWA-131 Wireless N Nano USB Adapter (Black).

  Note: (Workaround) : Since bluetooth is working absolutely fine, I use external bluetooth speakers. (Sorry, if you think this can't be workaround). 
- HDMI port (So not working dual display)

Very important Note !! 

Dell Lattitude 5590 ships with Samsung NVMe SSD which does not support due, so I replaced with Hynix M.2 SSD. Please check your configuration before proceeding.
Before installing wifi drivers for using DWA-131 Wifi USB adapter, you will have to disable SIP (System intergration Protection). 
This can be done in below steps:
  1. Restart and go into recovert mode (Be careful this is that recovery mode which runs without using external bootable BOOT EFI USB).
  2. MacOS installation screen will appears, ignore it and open Utilities > Terminal from top.
  3. Type csrutil status <-- to check current status
  4. Type csrutil disable <-- if status is enabled.
  5. Reboot the system in default mode and install the software by chris1111 mentioned above.
  6. Connect DWA-131 USB adapter and it will automatically scan, to show you available SSIDs.
  7. Connect yours and enjoy !!
  8. Optional but recommendded to enable the SIP after work is done.
  
Thanks!!

** About this build mac:**

![About](https://user-images.githubusercontent.com/50524850/87631318-bb31ba00-c754-11ea-9297-018be1cb8ac6.png)

![icons](https://user-images.githubusercontent.com/50524850/87631594-4612b480-c755-11ea-8ebe-58fe39d753ab.png)

![BT](https://user-images.githubusercontent.com/50524850/87631896-e668d900-c755-11ea-8c60-0df84f90a19a.png)

![Laptop-internal-Speakers](https://user-images.githubusercontent.com/50524850/87632051-39db2700-c756-11ea-9d6a-ed34e371717f.png)

![Uploading Brightness.png…]()

