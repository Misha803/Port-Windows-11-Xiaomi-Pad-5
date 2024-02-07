<img align="right" src="https://raw.githubusercontent.com/erdilS/Port-Windows-11-Xiaomi-Pad-5/main/nabu.png" width="425" alt="Windows 11 Running On A Xiaomi Pad 5">


# Running Windows on the Xiaomi Pad 5

## Get root 
> [!NOTE]
> **If you already have root just skip this step and go tothe next page**

### Prerequisites
- Brain
  
- [Android boot backup](/guide/English/1-partition-en.md#Make-a-backup-of-your-existing-boot-image)


## Patch boot 

- Copy ```boot.img``` file from ```platform tools``` folder to the tablet 


- Download and install [Magisk app](https://github.com/topjohnwu/Magisk/releases/latest) to tablet
  
-  Open Magisk app and click the Install button. Select ```Select and Patch a File``` option and find the ```boot.img``` file that you copyed to tablet. Click the ```Let's Go``` button and wait for the patching process to complete.
  
- Copy the ```magisk_patched......img```file from ```Downloads``` folder on tablet to ```platform tools``` folder on computer. 

- Reboot to fastboot
  
- Open command prompt in the platform tools folder 

 ## Flash patched boot 
```cmd
fastboot flash boot <magisk_patched.img>
```

### [Next step: Installing Windows](/guide/English/2-install-en.md)