# raspberry-pi-USA
first boot startup script to update most of the common changes made to a fresh Raspbian install

It will:
  run 'apt-get update' and 'apt-get dist-upgrade' to bring your installed packages up to date.
  install Samba to make it easier for your Windows PC to find it on your network by hostname.
  change locale and timezone information to US outside of raspi-config.
  change the keyboard layout to a US PC-104 keyboard
  enable the aliases for the 'ls' commands in .bashrc

It can also:
  change the ssh port to be used for communication.
  install a SSH-RSA key for auto-authentication on remote login.
  change the hostname of the Pi.
  
NOTICE: must be run as root!  use "sudo ./raspberry-pi-USA". Be sure to 'chmod 755' the script after downloading.

Some of the variables are set for my location and hardware, but can be easily modified.

I've worked out what was needed to prevent some of the error messages that pop up, so if you run the script
once and reboot, you should be set up for the typical US usage.
