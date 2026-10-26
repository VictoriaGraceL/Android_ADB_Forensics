# Troubleshooting record

## Slow Ubuntu installation

I reported starting around 5:15 PM and still waiting at 6:01 PM, approximately 46 minutes later. Some controls appeared gray or unresponsive. The installer eventually requested a restart and Ubuntu started successfully. The exact cause of the delay was not established.

## Virtual machine freeze

I encountered a freeze and powered the virtual machine off before restarting it. The exact cause was not established.

## Failed sudo password attempt

The package update screenshot shows one failed authentication attempt. Authentication subsequently succeeded and `sudo apt update` completed.

## ADB command not found

Installing `android-sdk-platform-tools-common` installed the common USB rules but left `adb` unavailable. I installed the `adb` package, after which the daemon started successfully.

## Wrong developer settings menu

I initially opened TalkBack developer settings. I then enabled system Developer options through the Build number entry and turned on USB debugging.

## No phone in the USB inventory

The initial `lsusb` output showed Linux root hubs and VMware devices. After the phone was connected to the Ubuntu virtual machine, Samsung Electronics Galaxy series appeared in MTP mode.

## Empty ADB device list

Several `adb devices` attempts returned an empty list. USB passthrough, system USB debugging, and phone authorization had to be completed before the connection worked.

## Unauthorized ADB connection

ADB briefly reported `unauthorized`. After accepting the phone USB debugging authorization prompt, it reported `device`.

## Long output and unsupported battery metric

The collection commands printed many lines and returned to the shell prompt. Battery measured charge statistics were reported as unsupported on this phone; other battery statistics were returned. Some evidence screenshots show the end of the output only.
