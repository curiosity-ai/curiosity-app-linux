# Curiosity for Linux

Curiosity is in early access for Linux. You can download the appropriate package file from the [releases page](https://github.com/curiosity-ai/curiosity-app-linux/releases/latest/), and manually install on your computer.

## Ubuntu and other Debian-based Linux
- Download the .deb file from the [latest release](https://github.com/curiosity-ai/curiosity-app-linux/releases/latest/)
- Check if you have libc6-dev installed. If not, install it using `sudo apt install libc6-dev`
- Install Curiosity using `sudo dpkg -i curiosity_VERSION.deb`
- To uninstall Curiosity (for example to install a new version), use `sudo dpkg -r curiosity` 

## Ubuntu Snap Store
In development - for now use the .deb file above.

## RedHat / CentOS
- Download the .rpm file from the [latest release](https://github.com/curiosity-ai/curiosity-app-linux/releases/latest/)
- Check if you have libc6-dev installed. If not, install it using `sudo yum install glibc`
- Install Curiosity using `sudo yum install curiosity_VERSION.rpm` (for RHEL 6+) or `sudo yum localinstall curiosity_VERSION.rpm` (for RHEL 5)

# Known Issues
###Missing libdl:
- You might need to install libc6-dev on your system. You can do that  by running `sudo apt install libc6-dev` (Ubuntu and other Debian-based Linux) or `sudo yum install glibc` (RHEL, CentOS)

## Updates not available
The update option is not yet supported on Linux. In order to update to a newer release, just download and install a new version - your data will be kept when you uninstall and install the new version.
