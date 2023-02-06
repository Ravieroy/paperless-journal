## Revert back to stock Android in Mi A2
---

^^==This tutorial assumes that, Ubuntu Touch is installed successfully, and now it is desired to revert to stock ROM. Read how to [[Flash Ubuntu Touch]] for more detail about basic procedure.==^^

## Requirements 
1. SDK Platform Tools ([Download Link](https://developer.android.com/studio/releases/platform-tools))
2. Stock Android ROM for Mi A2 ([Download Link](https://xiaomistockrom.com/xiaomi-mi-a2))
3. Xiaomi Mi A2 with TWRP recovery installed. 
4. Windows or Linux (preferably) PC. 

## Process
**Step 1 :** Boot the phone in [[Fastboot]] mode and connect it using *correct* USB cable. 

**Step 2 :** Open up a [[Terminal]] in the directory which has SDK platform tools. Check if the files `fastboot` and `adb` are executable or not. If not, type `chmod u+x fastboot` to make it executable. 

**Step 3 :** Once the phone is in [[Fastboot]] mode, check which slot is active. There are two slots A and B and you have to flash the ROM in both the slots. To check type,                  
```bash
./fastboot getvar current-slot
```

**Step 4 :** To change the slot type,
```bash
./fastboot --set-active=<a|b>
```
**Step 5 :** Once correct slot is picked, boot in TWRP using, 
```bash
./fastboot boot ~/Downloads/twrp-3.5.2_9-0-jasmine_sprout.img
```
**Step 6 :** In the TWRP menu, select **Advanced** > **ADBsideload** and then type in the [[Terminal]]
```bash
./adb sideload ./jasmine_sprout_stock_android9.zip
```

**Step 7 :** Once the flashing of the image in the slot is done, reboot the system in [[Fastboot]] and repeat the process *but change the slot from the earlier slot*.

Once this is done, simply reboot the system and stock ROM would be installed now. 

- For me the name of TWRP image was *twrp-3.5.2_9-0-jasmine_sprout.img* the stock ROM was *jasmine_sprout_stock_android9.zip*. The name should be changed accordingly.

---
- Sometimes the system might ask for factory reset. Use the volume keys to navigate the options and power key to select the choice.
- Any custom ROM can be flashed in the same fashion as above. [List of Best Custom ROM for Xiaomi Mi A2](https://www.getdroidtips.com/custom-rom-xiaomi-mi-a2/)
