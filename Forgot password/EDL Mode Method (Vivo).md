# Warning
- All user data will erased during this process.

# Tools Needed:
- [QPST (Qualcomm Product Support Tool)](https://raw.githubusercontent.com/AzimsTech/Android_Hacking/master/Tools/QPST.2.7.473.zip)
- [QDLoader HS-USB Driver](https://raw.githubusercontent.com/AzimsTech/Android_Hacking/master/Drivers/QDLoader_HS-USB_Driver.zip)

# General steps
1. Find & download the full firmware online for your devices. Example from this [website](https://www.firmware27.com/p/vivo.html).
2. Plug the phone into computer when it turned off and enter the EDL Mode. Search for test point picture for specific model online for refferences. [Example](https://www.google.com/search?q=vivo+y11+test+point)
3. Open QFIL program. Select the "**Select Build Type**" check box to "**Rat Build**". On "**Select Programmer**" section **Browse** the correct prog_emmc_firehose_xxxx.mbn file for your devices.
4. Click on **Tools** >> **Parition Manager** >> right-click **userdata** >> **Manage Partition Data** >> **Erase**. The program will output "**Finish Erase Data Block**" now unplug from the computer and turn on the device.
5. The device will start wiping data by itself during boot or you have to do it manually if it fails (sometimes may happen). 

# Additional Notes
- This method is tested on [Vivo Y11 (2019)](https://www.gsmarena.com/vivo_y11_(2019)-9925.php)
- This method only removes Funtouch OS's password lock & it doesn't bypasses Google FRP lock.
- To bypass FRP altogether you need to flash entire firmware instead (I'm not tested it yet 🤷‍♂️). To do that, skip step 4 and hit **Load XML** and select **rawprogram_unparse.xml** >> **patch0**. Hit **Download** and wait for it finished flashing. 

# Research
- [A set of QPST utilities and drivers - Lenovo forums](http://lenovo-forums.ru/tutorials/article/980-nabor-utilit-qpst-i-drayverov-dlya-proshivki-ustroystv-lenovo-na-baze-chipov-qualcomm-obnovlyaemaya/)
