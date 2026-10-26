# Screenshot index

All 33 images from the lab are included. Images have descriptive filenames; two sideways photographs have been rotated for readability.

## Figure 1 Authorized phone connection

[Authorized phone connection](01-authorized-phone-connection.jpg)

The clean adb devices result shows the connected phone with status device. This is the successful connection evidence for the first submission requirement.

## Figure 2 Android device properties

[Android device properties](02-android-device-properties.jpg)

The adb shell getprop command and property values are visible. This is the device information evidence for the second submission requirement.

## Figure 3 Installed application packages

[Installed application packages](03-installed-application-packages.jpg)

The terminal shows package identifiers and APK paths from adb shell pm list packages -f. This screenshot captures the end of the output and the returned shell prompt.

## Figure 4 System usage statistics

[System usage statistics](04-system-usage-statistics.jpg)

The terminal shows the end of the output collected with adb shell dumpsys usagestats. This image documents output completion; the command line and earlier usage records are outside this view.

## Figure 5 Battery statistics

[Battery statistics](05-battery-statistics.jpg)

The terminal shows battery statistics, constants, and the returned shell prompt. The measured charge statistics section reports that the specific measurement is not supported on this phone.

## Figure 6 System settings

[System settings](06-system-settings.jpg)

The terminal shows settings such as volume and Wi Fi calling values from adb shell settings list system, followed by the shell prompt.

## Figure 7 VMware installation account screen

[VMware installation account screen](07-vmware-installation-account-screen.jpg)

The VMware Easy Install screen requests Linux account information during virtual machine setup.

## Figure 8 Virtual machine configuration

[Virtual machine configuration](08-virtual-machine-configuration.jpg)

The VMware summary records a 30 GB split virtual disk, 4096 MB RAM, NAT networking, 2 CPU cores, and a USB controller.

## Figure 9 Ubuntu installation selection

[Ubuntu installation selection](09-ubuntu-installation-selection.jpg)

Install Ubuntu is selected in the Ubuntu installer inside VMware.

## Figure 10 Ubuntu installation photograph

[Ubuntu installation photograph](10-ubuntu-installation-photograph.jpg)

A second view of the Install Ubuntu selection documents the installer running on the Windows host through VMware.

## Figure 11 Ubuntu disk installation choice

[Ubuntu disk installation choice](11-ubuntu-disk-installation-choice.jpg)

The installer presents Erase disk and install Ubuntu and Manual installation. The disk being configured belongs to the virtual machine.

## Figure 12 Ubuntu encryption selection

[Ubuntu encryption selection](12-ubuntu-encryption-selection.jpg)

The encryption and file system screen shows No encryption selected. This photo has been rotated for readability.

## Figure 13 Optional Ubuntu software

[Optional Ubuntu software](13-optional-ubuntu-software.jpg)

The installer presents optional proprietary software and additional media format support.

## Figure 14 Ubuntu account creation

[Ubuntu account creation](14-ubuntu-account-creation.jpg)

The installer account screen records the local account setup stage.

## Figure 15 Ubuntu installation progress

[Ubuntu installation progress](15-ubuntu-installation-progress.jpg)

The Help and support installer screen shows the installation continuing.

## Figure 16 Later installation progress

[Later installation progress](16-later-installation-progress.jpg)

A subsequent progress screenshot records the extended installation wait.

## Figure 17 Package list update

[Package list update](17-package-list-update.jpg)

sudo apt update completes after one failed password authentication attempt. The output reports that package upgrades are available.

## Figure 18 USB rule package installation

[USB rule package installation](18-usb-rule-package-installation.jpg)

android-sdk-platform-tools-common and android-udev-rules are installed. This stage provides USB rules but does not by itself install the adb executable.

## Figure 19 ADB command initially missing

[ADB command initially missing](19-adb-command-initially-missing.jpg)

After the common platform tools package is installed, adb devices returns Command adb not found and suggests installing adb.

## Figure 20 ADB package installed

[ADB package installed](20-adb-package-installed.jpg)

The adb package and dependencies finish installing. The ADB daemon starts successfully, but no phone is listed yet.

## Figure 21 TalkBack developer settings

[TalkBack developer settings](21-talkback-developer-settings.jpg)

This screen is the TalkBack developer settings page. It was an initial navigation mistake when looking for the phone system Developer options.

## Figure 22 Second TalkBack settings view

[Second TalkBack settings view](22-second-talkback-settings-view.jpg)

A closer view of TalkBack settings documents the same navigation issue before enabling system USB debugging.

## Figure 23 Samsung phone identification

[Samsung phone identification](23-samsung-phone-identification.jpg)

About phone identifies the device as a Samsung Galaxy A13 5G with model SM-A136U.

## Figure 24 Android software identification

[Android software identification](24-android-software-identification.jpg)

Software information shows Android 13, One UI Core 5.1, and the Build number entry used to enable Developer options.

## Figure 25 USB connection to the virtual machine

[USB connection to the virtual machine](25-usb-connection-to-the-virtual-machine.jpg)

The USB connection dialog offers the running Ubuntu virtual machine as the target for the connected device.

## Figure 26 First ADB detection attempt

[First ADB detection attempt](26-first-adb-detection-attempt.jpg)

The ADB daemon starts, but the device list is empty. This photo has been rotated for readability.

## Figure 27 Repeated empty ADB device list

[Repeated empty ADB device list](27-repeated-empty-adb-device-list.jpg)

Another adb devices attempt returns an empty list before the phone connection is fully configured.

## Figure 28 USB inventory without the phone

[USB inventory without the phone](28-usb-inventory-without-the-phone.jpg)

The lsusb output lists Linux root hubs and VMware virtual USB devices, with no Samsung phone present.

## Figure 29 Samsung detected over USB

[Samsung detected over USB](29-samsung-detected-over-usb.jpg)

The later lsusb output includes Samsung Electronics Galaxy series in MTP mode, showing that Ubuntu now sees the phone over USB.

## Figure 30 USB detection before ADB authorization

[USB detection before ADB authorization](30-usb-detection-before-adb-authorization.jpg)

Although lsusb identifies the Samsung phone, subsequent adb devices attempts still return an empty list at this stage.

## Figure 31 USB debugging authorization prompt

[USB debugging authorization prompt](31-usb-debugging-authorization-prompt.jpg)

The phone has USB debugging enabled and displays the Allow USB debugging prompt with the computer RSA fingerprint.

## Figure 32 Phone data access prompt

[Phone data access prompt](32-phone-data-access-prompt.jpg)

The phone displays Allow access to phone data for the connected computer.

## Figure 33 ADB authorization transition

[ADB authorization transition](33-adb-authorization-transition.jpg)

The terminal shows the phone first as unauthorized and then as device after the debugging authorization is accepted.

