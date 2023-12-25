# CRAP

Note: This project was originally forked from [reynhout/chrx](https://github.com/reynhout/chrx).
The project has been completely rewritten since, and is now only a partitioning tool.
It does not include any feature to install an alternate operating system, you must do that yourself.

This tool works on all Chromebook models. See [documentation](https://chrultrabook.github.io/docs/docs/firmware/supported-devices.html).

## Usage

Running this script does not require you to have valid RW_LEGACY firmware installed,
but this is currently the recommended method for dual booting another operating system alongside ChromeOS.
See [MrChromebox's Firmware Utility Script](https://mrchromebox.tech/#fwscript) for installing RW_LEGACY firmware.

### Running the script

1. Ensure you're in developer mode and connected to WiFi.
2. Open VT2 using `[ Ctrl ] [ Alt ] [ → ]`, login as `root`
	- Note: the script cannot be run with crosh on any version of ChromeOS.
3. Run the script!
	- Run `bash <(curl https://raw.githubusercontent.com/chrultrabook/crap/master/crap)`
	- URL shortened version: `bash <(curl -L https://tinyurl.com/crap-cb-01)`
4. The script will walk you through the steps you need to take to make room for an alternate OS.

## Screenshots

CRAP - main menu

![Screenshot - CRAP - main menu](/screenshots/screenshot01.png)

CRAP - resizing stateful partition

![Screenshot - CRAP - resizing stateful partition](/screenshots/screenshot02.png)

## Notes

* We do NOT EVER use the KERN-C or ROOT-C partitions NO
