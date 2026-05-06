# How to set build.prop property via ADB
**Syntax:**

`setprop` `<property>` `<value>`

**Example:**
~~~
adb shell
su
setprop persist.adb.notify 0
~~~

# Build.prop Tweaks

| Property                    |Value | Description                                  | Documentattion    |
| ----                   | ---  | ----                                      | ------            |
| ro.config.low_ram | true/false |	turn off specific memory-intensive features | [Low RAM Device flag](https://source.android.com/devices/tech/perf/low-ram#flag) |
| persist.adb.notify |  0-1  | hide USB debugging notification | [UsbDeviceManager.java](https://android.googlesource.com/platform/frameworks/base/+/master/services/usb/java/com/android/server/usb/UsbDeviceManager.java#1180) |
| persist.camera.HAL3.enabled | 0-1 | enable Camera2 API on some devices | [Camera HAL3](https://source.android.com/devices/camera/camera3) |

# Research
- [How does adb shell getprop and setprop work?](https://stackoverflow.com/questions/40624222/how-does-adb-shell-getprop-and-setprop-work)
