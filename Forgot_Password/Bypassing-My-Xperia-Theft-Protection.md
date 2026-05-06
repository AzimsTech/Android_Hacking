# Bypassing My Xperia Theft Protection (MXTP)
![cover](https://i.imgur.com/HB6jDjk.jpg)

# Tools
- [Flashtool + Flashmode Driver ](http://www.flashtool.net/downloads.php)

# Steps
1. Find **FTF Firmware** & **Lock Remove File** for specific device online. Place both files under `%UserProfile%\.flashTool\firmwares`
~~~ 
Example:

E6553_32.2.A.0.305_R7C_CustomizedVN.ftf     //  Firmware
E6553_32.2.A.0.305_R7C_RemoveLock.ftf       // Lock Remove File
~~~


2. Open **Flashtool** >> **Flash Device** >> **Flashmode** >> Start flashing the **Firmware** first:
![example1](https://i.imgur.com/lwr8GJO.png)
3. Flash the **Remove Lock** file next:
![example2](https://i.imgur.com/EbYl993.png)

4. Turn on the device 

## Every step must be done in 15-20 seconds:
5. Get to the home screen by finishing the first setup as quick as possible. If fail, reboot & try again.
6. Switch to Guest account (**Settings**>> **Users** >> **Guest**)
7. Remove Guest account (**Settings**>> **Users** >> **Remove guest**). Reboot.
8. Connect to a Wifi. If fail, reboot & try again.
9. Activate *my Xperia Protection* (**Settings** >> **Security** >> **Protection by my Xperia** >> **ACTIVATE** >> Login with **any Google accounts**) . If fail, reboot & try again.
10. Deactivate *my Xperia Protection* (**Settings** >> **Security** >> **Protection by my Xperia** >> **DEACTIVATE** >> Login with **previous Google accounts**) . If fail, reboot & try again.
11. **POWER OFF** will be popped out. Press that.
12. Now the device no longer ties to **my Xperia Protection** after we turn on.

# Additional Notes
- Do not use a long email password.
- Disable 2FA & Recovery email/phone inside Google account.
- Check your email to verify new sign-in activity.
- Create a Settings shortcut.
- This method is tedious and time-consuming. Practice and patience is the key.
- It is recommended to flash an official firmware after these steps.

# Resources
- [Flashtool by Androxyde](http://www.flashtool.net/downloads.php)
- [FTF Firmware & Lock Remove file downloads](https://vietfones.vn/forum/threads/sony-ftf-firmware-ftf-lock-remove-file-setool-file-download-here.1589959/)
- [4pda.ru forums](http://4pda.ru/forum/index.php?showtopic=677035&st=740#entry50786588)
- [Youtube video (Spanish)](https://www.youtube.com/watch?v=6TLrbmlY2DI)
