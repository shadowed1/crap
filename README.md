# CRAP

Note: This is a project forked from [reynhout/chrx](https://github.com/reynhout/chrx).
We are simply updating it to remove the Linux installation feature as it is outdated.
Instead, CRAP is only a partitioning tool for ChromeOS.
This does not have the Linux Install feature, you will have to linux yourself.

This tool works on all Chromebook models. See [Documentation](https://chrultrabook.github.io/docs/docs/firmware/supported-devices.html).

## Usage

1. **Enable [Developer Mode](https://chromium.googlesource.com/chromiumos/docs/+/HEAD/debug_buttons.md)**
    * For most chromebook models, enter recovery mode by pressing `ESC+Refresh+Power`, then press CTRL+D, then Enter.
2. **Boot ChromeOS and open Terminal**
    * Press `CTRL+D` at the "ChromeOS is missing or damaged" (or "OS verification is OFF") screen
	* DO NOT PRESS "Enable debugging features"
    * Configure Wi-Fi and log in (Guest account is fine)
    * Open VT2 using `[ Ctrl ] [ Alt ] [ → ]`, login as `chronos` (no password)
3. **Update firmware, if necessary**
    * Run MrChromebox's [Firmware Utility Script](https://mrchromebox.tech/#fwscript)
    * Select `Install/Update RW_LEGACY Firmware`
4. **Download and run CRAP**
    * `bash <(curl https://raw.githubusercontent.com/chrultrabook/crap/master/crap)`
	* *todo: url shortener or better host?*
5. **Follow on-screen instructions** to allocate storage space for Linux
    * CRAP will suggest dedicating as much space as possible to Linux, and as little as necessary for ChromeOS. Choose your allocation ratio according to your personal requirements and preferences!

## Notes

* We do NOT EVER use the KERN-C or ROOT-C partitions NO
