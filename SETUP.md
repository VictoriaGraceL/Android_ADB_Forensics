# Setup and collection

## 1. Prepare the virtual machine

Create an Ubuntu 64 bit virtual machine in VMware Workstation. The recorded configuration was a 30 GB split disk, 4096 MB RAM, 2 CPU cores, NAT networking, and a USB controller. Boot the Ubuntu installer and select **Install Ubuntu**. Complete the installer using the virtual disk, create a local account, and restart when prompted.

The erase disk option applies to the virtual machine disk in this setup. The installation record includes the disk selection, no encryption selection, account setup, and progress screens.

## 2. Install ADB

Open an Ubuntu terminal and run each command separately:

```bash
sudo apt update
sudo apt install android-sdk-platform-tools-common
sudo apt install adb
```

The common package installed USB rules in this lab. The separate `adb` package provided the missing ADB executable.

## 3. Prepare the Samsung phone

1. Open **Settings > About phone > Software information**.
2. Tap **Build number** seven times and authenticate if requested.
3. Return to Settings and open the system **Developer options**.
4. Enable **USB debugging**.
5. Connect the phone using a USB data cable and keep it unlocked.
6. In VMware, connect the Samsung USB device to the Ubuntu virtual machine.
7. Accept the **Allow USB debugging** prompt for this lab computer. Accept the phone data access prompt if shown.

The developer settings inside TalkBack are a different menu. Use the phone system Developer options.

## 4. Verify detection

```bash
lsusb
adb devices
```

The USB list should include Samsung. The successful ADB result shows the phone identifier followed by `device`. If it says `unauthorized`, unlock the phone and accept the debugging authorization prompt.

## 5. Collect information

Run the following separately and capture each command with its output where possible:

```bash
adb shell getprop
adb shell pm list packages -f
adb shell dumpsys usagestats
adb shell dumpsys batterystats
adb shell settings list system
```

Long output is expected. Scroll up to capture the command and relevant results. The return of the Ubuntu shell prompt indicates that the command has finished. The collected statistics depend on the device and its Android version.

## 6. Finish

Save the screenshots and report. When finished with the lab, disconnect the phone and turn off USB debugging if it is no longer needed.
