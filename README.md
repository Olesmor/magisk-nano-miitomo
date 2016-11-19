Nano-Miitomo Magisk Module
===========================

Miitomo is the first mobile application developed by Dena for Nintendo.

In versions 1.0.0 - 1.1.3 Miitomo was locking out users on rooted devices,
starting with version 1.2.0 this restriction was removed by Dena. But still
Miitomo checks for the system property

	ro.debuggable

if the value is '1', Miitomo will crash on purpose. So what this module does,
is to use the shiny new 'resetprop' introduced in Magisk v9 to set the value
of 'ro.debuggable' to '0'.

This Magisk Module is meant for users that can't or don't want to use Xposed,
Xposed users can use my [SecurityBypasser](https://github.com/Nanolx/MiitomoSecurityBypasser) Xposed module, instead.

Download 'magisk-nano-miitomo-release.zip' from on github (or create a zip file
from the git repo) and flash the zip file using TWRP or install it using Magisk
Manager. After you've installed it, reboot the device and Miitomo will work.

For further information refer to:
* [Magisk](http://forum.xda-developers.com/apps/magisk/official-magisk-v7-universal-systemless-t3473445)
* [Miitomo](https://miitomo.com/)
