# GMenuNext

[GMenuNext](https://github.com/pingflood/GMenuNext/) is a fork of [GMenu2X](http://mtorromeo.github.com/gmenu2x) developed to Retrogame RS-97, released under the GNU GPL license v2.


## Installation

Unpack the [Release](https://github.com/pingflood/GMenuNext/blob/master/dist/rs97/GMenuNext.zip) over your current GMenu2X directory, or download the [latest binary](https://github.com/pingflood/GMenuNext/raw/master/dist/rs97/gmenu2x/gmenu2x) and replace it in your device.

(Re)Boot your device and enjoy [GMenuNext](https://github.com/pingflood/GMenuNext/).


## Changelog

**2018-04-26**
* Add some system information in About screen;
* About screen using about.txt

**2018-04-25**
* Save screenshot in a ./screenshots
* First adjust in battery indicator based in data provided by Battery Logging. Thanks to @Valenhir, @m1024 and @Jutley for logging and sharing battery data. ;)

**2018-04-24**
* Fixed incorrect brightness when returning from suspend mode;
* Dynamic fill the icon tray;
* Added option to auto hide a MessageBox;
* Use MessageBox to draw some messages;
* Save screenshot with combo [X] + [BUTTON_R];
* Mute/unmute with combo [X] + [TRIGGER_L];
* Fix in DekUI messagebox color;
* Screenshot function is global
* Brightness control is global

**2018-04-23**
* Fixed the Log Viewer;
* Added default values for brightness and global volume;
* New poweroff menu;
* New brightness slider control;
* New battery logger screen;
* New linear fit for battery level measurements (waiting for logs to improve);
* Rearranged how all input buttons are handled in main menu;
* Added option to customize the inactive timeout to suspend. Values can be set set between 10 to 300 seconds;
* Improved how to trigger power off and suspend via power button:
     * If hold the power button for ~1s, it will suspend the device;
     * If hold the power button for ~2.5s, power off menu will pop up;
* When waking up from suspended state, a press in power menu should wake up the device with at least 10% of brightness level;
* Rearranged in "core" of the main menu where it redraws the screen. Prevent redraw screen while in "suspend" mode.
* Absolute path resolving in filelister; Prevents (?) buffer overflow after browsing a lot of files and allow resolving relative paths.

**2018-04-20**
* New main menu layout, with a section bar on the left and items in list, inspired in [concept designed by @m1024](http://boards.dingoonity.org/ingenic-jz4760-devices/gmenunext-let's-make-gmenu-great-again!/msg177170/#msg177170);
* Retouched every screen to make all system cohesive;
* Alternative selector browser, allowing you to load previews of your games if selector previews is set;
* Navigate page up/down with directional left/right;
* New variables for skin designers;
* New set of "Next" skins by @m1024.


## [How to have previews in Selector Browser](http://boards.dingoonity.org/ingenic-jz4760-devices/gmenunext-let's-make-gmenu-great-again!/msg177392/#msg177392)

* Select the link you want to edit and press "menu";
* Edit the link;
* Configure the link to match your directory structure. Important fields:
	* Selector Directory: The directory of your roms
	* Selector Browser: Enable selector before launching the app
	* Selector Filter: Filter extensions to be shown in the selector. Separe multiple extensions with commas.
	* Selector Screenshots: The directory of the screenshots/preview of your roms. It can be different than your roms directory.
* The name of the file of rom and preview have to be exactly the same. Suported image types are .png or .jpg;


## How to create battery logs

To get data of your battery charge and discharge cycle:
* Enter the Battery Logger;
* Do a full charge;
* After charged, remove the cable;
* Stay in this screen and wait until it discharges totally;

Repeat how many times you wish and can.

New data will be printed on screen every minute and will be saved in file **battery.csv** located in **gmenu2x** folder.

The fields logged are:
* Time: Time in milliseconds since GMenuNext started;
* BatteryStatus: Computed battery status, from 0 (discharged) to 4 (charged) and 5 (charging);
* BatteryLevel: Raw battery level as given by system.


## Controls

All controls are being revised. Here's the legacy GMenu2X control mapping:
* X, Stick left: Goes up one directory in file browser.
* X: Cancel action.
* B, Stick press: Launch selected link / Confirm action.
* L, R: Switch between sections - PageUp/PageDown on lists.
* Y: Bring up the manual/readme.
* VOLDOWN: Decrease cpu clock.
* VOLUP: Increase cpu clock.
* VOLDOWN+VOLUP: Reset clock.
* A+VOLDOWN: Decrease volume for the selected link.
* A+VOLUP: Increase volume for the selected link.
* A+VOLDOWN+VOLUP: Reset volume for the selected link.
* SELECT: Bring up the contextual menu.
* START: GMenu2X options.


## Contacts

I want to thanks [@m1024](https://boards.dingoonity.org/profile/m1024/) and [@jutley](https://boards.dingoonity.org/profile/jutley/) for all the support they are giving, testing and reporting bugs.

## Contacts

GMenu2X Copyright (c) 2006-2010 [Massimiliano Torromeo](mailto:massimiliano.torromeo@gmail.com); GMenuNext 2018 by [@pingflood](https://boards.dingoonity.org/profile/pingflood/); Skin PS4, PSNext, PSNextDark and Zelda by [@m1024](https://boards.dingoonity.org/profile/m1024/)

Visit the [Dingoonity thread](https://boards.dingoonity.org/ingenic-jz4760-devices/gmenunext-let's-make-gmenu-great-again!/) and the [Discord channel](https://discord.gg/hvR5vK6)!

[GMenu2X](http://mtorromeo.github.com/gmenu2x) homepage for more info.
