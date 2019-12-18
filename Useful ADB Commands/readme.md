# Useful ADB + Shell Commands
- [ADB Server Basics](#ADB-Server-Basics)
- [Copy files to/from a device](#Copy-files-to/from-a-device)
- [Install an app](#Install-an-app)
- [Android package manager (pm)](#Android-package-manager-(pm))
- [Research](#Research)

## ADB Server Basics
~~~ 
adb devices // To confirm device is connected
adb kill-server // To reset ADB host
~~~
## Copy files to/from a device
**To copy `from` a device:**

`adb` `pull` `<device>` `<computer>`

**To copy `to` a device:**

`adb` `push` `<computer>` `<device>`

**Example:**
~~~
adb push foo.txt /sdcard/foo.txt
adb pull /sdcard/bar.txt C:\
~~~

## Install an app
`adb` `install` `path_to_apk`

**Example:**
~~~
adb install "C:\com.google.android.youtube.apk"
~~~

# Android package manager (pm)
**Get list of `system apps` on the device:**
```bash
adb shell "echo 'apps:' && pm list packages -f | grep /system/app/ | sed 's/.*=/  - /'"
```
**Directories:** System apps / pre-installed-bloatware-apps are stored in ``/system/app`` with privileged apps in ``/system/priv-app``

**Formatting Regex:** `s/.*=/  - /`

## Remove application command
```bash
pm uninstall --user 0 app
```
**Option/switches:** 

**-k**: To keep the data and cache directories around after package removal.

**Example:**
```bash
pm uninstall -k --user 0 com.facebook.system
pm uninstall -k --user 0 com.facebook.services
pm uninstall -k --user 0 com.facebook.katana
pm uninstall -k --user 0 com.facebook.appmanager
```

## Activate USB Tethering 
**This depends on the Android version:**

~~~
service call connectivity 32 i32 1 on Ice Cream Sandwich (4.0)
service call connectivity 33 i32 1 on Jelly Bean (4.1 to 4.3)
service call connectivity 34 i32 1 on KitKat (4.4)
service call connectivity 30 i32 1 on Lollipop (5.0)
service call connectivity 31 i32 1 on Lollipop (5.1) 
service call connectivity 30 i32 1 on Marshmallow (6.0)
service call connectivity 41 i32 1 on Samsung Marshmallow (6.0)
service call connectivity 33 i32 1 on Nougat (7.0)
service call connectivity 39 i32 1 on Samsung Nougat (7.0)
~~~

**For Android 8 & above:**
~~~
service call connectivity 34 i32 1 s16 text (8.0/8.1)
service call connectivity 33 i32 1 s16 text  (9.0)
~~~

**Example (Android 8.1):**

~~~
adb shell "su -c 'service call connectivity 34 i32 1 s16 text'"
~~~


# Research
- [Official ADB Documentation](https://developer.android.com/studio/command-line/adb)
- [Calling Android services from ADB shell](http://ktnr74.blogspot.com/2014/09/calling-android-services-from-adb-shell.html)
- [Is it possible to USB tether an android device using adb through the terminal?](https://stackoverflow.com/questions/20226924/is-it-possible-to-usb-tether-an-android-device-using-adb-through-the-terminal)
- [AdbCommands](https://gist.github.com/Pulimet/5013acf2cd5b28e55036c82c91bd56d8)


