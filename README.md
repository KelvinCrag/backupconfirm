# backupconfirm
**DISCLAIMER**: Google warns that ADB backup and restore may be removed in a future Android release.

## Summary
This script uses a system app called **com.android.backupconfirm** to backup and restore your stored data at a time convenient for you.

## Features
* [X] Lightweight simple script. Concise and optimised.
* [X] Ability to backup and restore data without installing an app or the use of internet.
* [X] Improved screen feedback on what is happening currently.
* [X] noob-friendly

## How to use it 
- Enable *Developer Options* on your smartphone.
- Turn on *USB Debugging*.

### LINUX
- Install *Android platform tools* with your package manager :

 	Debian Base : 
 	```console
	apt-get install android-sdk-platform-tools
 	```
 	Arch-Linux Base :
 	```console
 	pacman -S android-tools
	```

- use **adb backup -apk -shared -all -f <filepath>/backup.ab** to backup and **adb restore <filepath>/backup.ab** to restore


### WINDOWS
- Install [ADB](https://dl.google.com/android/repository/platform-tools-latest-windows.zip). If you want ADB support everywhere on your PC, you need to add the path of the ADB folder in the system variables (see [this](https://www.xda-developers.com/adb-fastboot-any-directory-windows-linux/)).

- Go to the [release section](https://github.com/KelvinCrag/backupconfirm/releases) and download the lastest release.

- Put .bat in the same folder of installed adb. By default it is c:/adb/platform-tools et voilà !



