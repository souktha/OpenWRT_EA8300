# OpenWRT_EA8300
OpenWRT Chaos Calmer for Linksys EA8300 Max-Stream AC2200 Wi-Fi router

To install OpenWRT Chaos Calmer to the router,

- Login to the router that is currently running Linksys firmware via its Web UI with the web browser (Chrome/firefox etc).

- Click on *connectivity* on the left panel below *Router Settings*. The *connectivity* will show up. On the right pane, there is 
  *Router Firmware Update*. Under it, there is *Manual* box. Select *Choose File* where you can pick the file you downloaded
  from my git repository. This is the file to flash into the router.

- After choosing file (LINKSYS_EA8300-openwrt.img), choose *start* to program the flash. Flashing will be on the partitions
  that is not the current set of root file system (Linksys). It will be automatically chosen for you. The OpenWRT image
  contains both kernel and rootfs so everything is OpenWRT.

- Click *yes* to continue on *Important* pop-up warning message.

- Firmware updating process will take place and the EA8300 router will reboot. This process should take less than 30s.
  Click *ok* when pop-up message tells you that it is rebooting (to new OpenWRT firmware).


Default SSIDs for this firmware are "OpenWrt_EA8300" and "OpenWrt_EA8300_5g" with the default IP address 192.168.2.1. It is open-access. Use host PC to connect to either one of these SSIDs to configure the router via telnet or via WebUI.
