# CRAP

Note: This is a project forked from ([github.com/reynhout/chrx](https://github.com/reynhout/chrx)). We are simply updating it to work with modern chromebooks. This does not have the Linux Install feature, you will have to linux yourself. 

| | |
| ------------ | ---------- |
|**works on**|All Chromebook models. See [Docs](https://chrultrabook.github.io/docs/docs/supported-devices.html).|




<a name="usage"></a>
## usage

Installing Linux via **chrx** onto a new (or freshly recovered) Chromebook

- The first phase reserves space on your storage device for
the new operating system, **and then reboots**.



<a name="step-by-step"></a>
### step-by-step

1. **Enable [Developer Mode](http://www.chromium.org/chromium-os/developer-information-for-chrome-os-devices)**
    * (for most models, press `ESC+F3(Refresh)+Power`)
1. **Boot ChromeOS and open Terminal**
    * Press `CTRL+D` at the white "ChromeOS is missing or damaged" (or "OS verification is OFF") screen
    * Configure Wi-Fi and log in (Guest account is fine)
    * Open ChromeOS Terminal by pressing `CTRL+ALT+T`, and entering `shell` at the prompt
1. **Update firmware, if necessary** -- see [chromebooks](#chromebooks)
    * Open Virtual Terminal 2 using ```[ Ctrl ] [ Alt ] [ → ]```
    * run MrChromebox's Firmware Utility Script see ([Firmware Script](https://mrchromebox.tech/#fwscript))
    * Select ```Install/Update RW_LEGACY Firmware```
1. **Download and run chrx**
    * *add install link here*
1. **Follow on-screen instructions** to allocate storage space for Linux
    * CRAP will suggest dedicating as much space as possible to Linux, and as little as necessary for ChromeOS. Choose your allocation ratio according to your personal requirements and preferences!


<!--
<a name="advanced-usage"></a>
### advanced usage

You may choose to host or cache these installation files yourself.
There are many good reasons to do so, especially if you'll be doing
a large number of installations. However, setup can be somewhat more
complicated, and instructions are outside the scope of this README.

To point **chrx** at your cache, just set the `CHRX_WEB_ROOT`
environment variable before running the `chrx` script, like this:

```
export CHRX_WEB_ROOT="http://myserver/chrx"
cd ; curl -O $CHRX_WEB_ROOT/go && sh go
```
-->
