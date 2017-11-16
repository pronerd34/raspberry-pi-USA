# raspberry-pi-USA
first boot startup script to change locale information to US outside of raspi-config.

The variables are set for my location and hardware, but can be easily modified.

The first section (lines 2-7) set some environmental variables so that dpkg-reconfigure doesn't complain later.

the second section (lines 8-11) creates /etc/timezone with a defined timezone, then sets that by configuring tzdata.

the third section (lines 12-21) enables en_US.UTF-8 as a locale and disables en_GB.UTF-8, then sets en_US.UTF-8 as the default locale.

the fourth section (lines 22-27) change the variables in /etc/default/keyboard to match the typical US PC keyboard.

I'm still working to determine what's needed to prevent some of the error messages that pop up, but if you run the script once and reboot
twice, you should be set up for the typical US setup.
