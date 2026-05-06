# Bypassing FRP on Samsung A02s (EDL Method)

 ![cover](cover.png)

> [!WARNING]
> **Disclaimer:** Use these steps only on devices you own. Unauthorized bypassing of security features is illegal.

> [!TIP]
> Do a factory reset if you haven't already.

# Downloads
- [prog-emmc-firehose-8953-ddr.mbn](./prog-emmc-firehose-8953-ddr.mbn)
- [QPST (Qualcomm Product Support Tool)](../../Tools/QPST-2.7.473.zip)
- [QDLoader HS-USB Driver](./QHSUSB-Drivers.7z)
# Step by Step

1. **Entering EDL mode**
    - Turn off & disamssamble back cover
    - Unscrew black plastic cover on top of the mainboard
    - Short two pins near camera module:  
    <a href="EDL-pinout.jpg"> <img src="EDL-pinout.jpg" width="300"></a>  
    - Plung the phone to the computer while shorting those two pin
    - Extract and Install the **QDLoader HS-USB Driver**

2. **Erasing FRP**
    - Download and install **QPST**
    - Search and Run **QFIL**  
    <a href="run-QFIL.png"> <img src="run-QFIL.png" width="300"> </a>  
    - Follow video below:
    - Your phone will reboot

https://github.com/user-attachments/assets/fcf7d4c1-14d6-4090-a3c4-6902156d93ff  

    
> [!NOTE]
> Tested on Samsung Galaxy A02s Android 12 (17 Nov 2025)
