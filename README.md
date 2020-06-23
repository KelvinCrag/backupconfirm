# backupconfirm
**DISCLAIMER**: Google warns that ADB backup and restore may be removed in a future Android release.

## Summary
This script uses a system app called `com.android.backupconfirm` to backup and restore your stored data at a time convenient for you.

## Features
* [X] Lightweight simple script. Concise and optimised.
* [X] Ability to backup and restore data without installing an app or the use of internet.
* [X] Improved screen feedback on what is happening currently.
* [X] noob-friendly

## How to use it 
- Enable *Developer Options* on your smartphone.
- Turn on *USB Debugging* from the Developer Options.<p>
<details>
<summary>LINUX</summary>

- Install *Android platform tools* and *qpdf* on your PC :

Debian Base :
```bash
$ sudo apt install android-sdk-platform-tools qpdf
```
Arch-Linux Base :
```bash
$ sudo pacman -S android-tools qpdf
```
Fedora :
```bash
$ sudo yum install android-tools qpdf
```
- Use `adb backup -apk -shared -all -f <filepath>/backup.ab` to backup and `adb restore <filepath>/backup.ab` to restore.
</details>
</p>

<p>
<details>
<summary>MAC OS</summary>

- Install [Homebrew](https://brew.sh/)
- Install *Android platform tools* and *qpdf*
```bash
$ brew install android-platform-tools qpdf
```
- Use `adb backup -apk -shared -all -f <filepath>/backup.ab` to backup and `adb restore <filepath>/backup.ab` to restore.
</details>
</p>

<p>
<details>
<summary>WINDOWS</summary>


- Download [android platform tools](https://dl.google.com/android/repository/platform-tools-latest-windows.zip) and unzip it somewhere. [Add the folder to your PATH](https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/).
- [Install USB drivers of your device](https://developer.android.com/studio/run/oem-usb#Drivers)
- Check your device is detected :
```batch
 adb devices
```
- Go to the [release section](https://github.com/KelvinCrag/backupconfirm/releases) and download the lastest release.

- Put .bat in the same folder of installed adb if you don't have adb support everywhere in your PC. By default, it is `c:/adb/platform-tools`

```
backupconfirm.bat
```
</details>
</p>

- adiós amigos
 
