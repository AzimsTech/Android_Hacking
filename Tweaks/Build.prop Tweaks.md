# How to Add The Line to build.prop from ADB
Example:
~~~
adb shell
su
setprop persist.adb.notify 0
~~~

# Build.prop Tweaks

| Key                    | Description                                  | Documentattion    |
| ----                   | -------                                      | ------            |
| ro.config.low_ram=true |	turn off specific memory-intensive features | [Low RAM Device flag](https://source.android.com/devices/tech/perf/low-ram#flag) |
| persist.adb.notify=0   | hide USB debugging notification | [UsbDeviceManager.java](https://android.googlesource.com/platform/frameworks/base/+/master/services/usb/java/com/android/server/usb/UsbDeviceManager.java#1180) |

