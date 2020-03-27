# Formatting FRP Partition on Mediatek Devices

# Tools
- [MTK Android USB Driver](Drivers/MTK_Android_USB_Driver.zip) 
- [SP Flash Tool](Tools/SP_Flash_Tool_exe_Windows_v5.1916.00.000.zip)

# Steps
1. Find **factory firmware** for specific device online.
2. Open **SP Flash Tool** & browse for device's **scatter** file.
3. Go to the **Format** tab , then mark **Manual Format Flash**.
4. Set the necessary values (refer to the scatter file)
![example](https://i.imgur.com/Tw9y7IX.png)
5. click **Start** , connect the device. At the end there will be a small window " **OK** ".
6. Click on "Start".
7. Connect the switched off phone to the computer.

# Caveat
Didn't work on some newer MTK (MediaTek) devices as it requests an authentication certificate to flash.
Example: Redmi 6A - it require special Xiaomi account (authorized mi account)
