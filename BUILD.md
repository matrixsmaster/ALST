# How to build ALST

## Prerequisites

1. A VM or physical machine with Windows 98 / 2000 / XP / 7. Alternatively, any modern \*NIX system with WINE (e.g., Linux Mint with `wine` package installed)
1. A copy of **Borland C++ Builder 6** (later versions might or might not work, I haven't tested them)
1. **MSM's Code Eye** tool from [GitHub](https://github.com/matrixsmaster/CodeEye) - you can either download a binary release or use previous two items to build your own copy from source

## Building

1. Open **MSM's Code Eye** and press *F3* to open a mix file
1. Select the ALST *MixProj* file from this repo
1. Press *F4* to run automatic deobfuscation (it'll only take a second or two)
1. Press *F5* to extract (or as I call it "explode") all files from the now-deobfuscated MixFile
1. Select (or create) any directory you want the files to be in, and press OK (**WARNING:** Existing files will be overwritten!)
1. Open **Borland C++ Builder 6** and press *Ctrl+F11* to open the project from the directory where you previously exploded the files
1. Click "OK" in the pop-up about missing \*.res file
1. Go to "Project" menu, then click "Options" (or simly press *Shift+Ctrl+F11*)
1. Go to "Application" tab and press "Load icon..." button
1. Select "Icon1.ico" file from this repo
1. Go to "Compiler" tab and press on "Release" button to make sure all settings are in Release configuration
1. Click OK to close the project options window
1. Press *Shift+Ctrl+S* to save everything
1. Press *F9* to start building the project; it may take a few minutes, depending on the speed of your machine
1. Enjoy!

## Troubleshooting

In general, build process is based on a tool which is frozen in time. Therefore, if ALST compiles on one machine, it **will** compile anywhere.
However, some compatibility issues of the toolchain itself might occur due to the fact we're using 20+ years old software (BCB6) on modern machines.

Here's the list of known compatibility issues:

|Environment HW|Environment SW|Symptoms|Mitigation|
|:-------------|:-------------|:-------|:---------|
|Intel Core-i9 CPU (12th gen upwards)|VirtualBox 6.1 or later with Windows XP as guest OS|Random freezes of C++ Builder and in some cases BSODs if you attempt to compile any substantial project|Move your VM to a machine with better CPU or use QEMU with TCG acceleration|
