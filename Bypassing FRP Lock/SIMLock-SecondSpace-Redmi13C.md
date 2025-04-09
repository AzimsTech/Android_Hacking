# Bypassing FRP on Xiaomi Redmi 13C (HyperOS/MIUI14)
![13c](https://gist.github.com/user-attachments/assets/36ff679d-4226-4cf3-8385-b055616ba0fd)

> [!WARNING]
> **Disclaimer:** Use these steps only on devices you own. Unauthorized bypassing of security features is illegal.

---

## Tools

- A SIM card with SIM lock turned on.
- A second Android phone for file transfer:
   - **Activity Launcher** (Download from Google Play)
   - **ShareMe App** (Download from Google Play)

---

## Steps

1. **Wi‑Fi & SIM**  
   - Connect to Wi‑Fi.  
   - Insert a SIM card with a SIM lock.  
   - "Enter the SIM PIN" screen will appear; lock the phone and remove the SIM.

2. **Open Settings**  
   - Turn on the screen, swipe down, and tap the **Settings** icon.
     ![notification tray](https://gist.github.com/user-attachments/assets/1823a366-578e-40c6-a220-86ddfab59cb0)


3. **Google Help & Share**  
   - Open **Google** settings.  
   - Tap the **“?” (Help)** icon.  
   - Open a help article and tap **Share Help** → Select **ShareMe**.

4. **Prepare Second Phone**  
   - On the second device, open **ShareMe** and tap **Receive**.
   - The QR code will appear here.
5. **Send File & Launch Activity**  
   - On the Redmi 13C, scan the QR code.  
   - On the second phone, tap **Send File** and choose **Activity Launcher**.
   - Install & Run Activity launcher on the Redmi 13C
   - In Activity Launcher, search for:  `Second Space`
   - Tap on
     `com.miui.securityspace.ui.activity.PrivateSpaceMainActivity`  
   - Tap to launch **Second Space** setup.

7. **Activate & Wipe**  
   - Complete Second Space setup.  
   - Power off, then boot into Recovery Mode (Volume Up + Power).  
   - Select **Wipe Data** and confirm.  
   - Reboot—the FRP lock should be bypassed.

---

> [!NOTE]
> Tested on Redmi 13C (4 January 2025)
