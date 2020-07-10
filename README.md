# macOS.Catalina.Hackintosh.on.Dell.Lattitude.5590
MacOS Catalina Hackintosh Built on Dell Lattitude 5590 Model 

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



What is not working ?

- Wifi 
  Note: (Workaround) : Bought a new USB Wifi dongle and installed the latest version of software from https://github.com/chris1111/Wireless-USB-Adapter,
  I am using D-Link DWA-131 Wireless N Nano USB Adapter (Black).
- Audio on internal laptop speaker
  Note: (Workaround) : Since bluetooth is working absolutely fine, I use external bluetooth speakers. (Sorry, if you think this can't be workaround). 


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


thanks!!

