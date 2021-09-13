Install Magisk On Official Android Emulator
===========================================

Works on Android API 30 only

0. Buy M1 Mac!
1. For patching the ramdisk with magisk, your AVD must be already created
2. Make sure you backup the untouched `ramdisk.img` from `<sdk_home>/system-images/<platform>/*/ramdisk.img`. You will need it everytime you want to patch ramdisk with magisk (for the first time and also for subsequent magisk updates).
3. Clone this repository and copy the original `ramdisk.img` into the clone's folder.
4. Start the newly created AVD.
5. Execute `patch.sh` to install Magisk on the ramdisk.img 
6. When finished, copy the patched `ramdisk.img` back to AVD directory.
7. Power off and restart (cold start) the emulator
8. Enjoy Magisk :)

Sources
=======
busybox binary : https://github.com/Magisk-Modules-Repo/busybox-ndk

Notes
=====
| Emulator Version | command-line patch | manager patch
| ---- | ---- | ---- |
| Android S | Canary (22001) | Canary (22001, w/ built-in `su`) |
| Android 22 - 30 | Canary (22001) | 21.4 (w/ manager 8.0.7) |

MagiskManager 8.0.7: https://github.com/topjohnwu/Magisk/releases/download/manager-v8.0.7/MagiskManager-v8.0.7.apk

Magisk 21.4 channel url: https://bit.ly/304BAei (https://github.com/topjohnwu/magisk_files/blob/b0694fad863d3a15c6a2276b1061a280ece80ed7/stable.json)

Magisk 22001 Canary: https://github.com/topjohnwu/magisk_files/raw/c34d91edab45e140753e1256f2b694eed90d2dcc/app-debug.apk
