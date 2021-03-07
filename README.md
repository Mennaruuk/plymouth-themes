
<h1 align="center">🚀 Rocket Theme 🚀</h1>


<p align="center">
Get that combusting rocket animation found in Pop!_OS installation right on your splash screen.</a>

<p align="center">
For Debian-based distros only!
</p>

<p align="center"> (just because I have no idea how to code or do anything Linux. I'm weird.) </a>
</p>

<p align="center">
  <img src="https://i.imgur.com/4ofcFSr.gif" />
</p>

### What is Plymouth?

[Plymouth](http://www.freedesktop.org/wiki/Software/Plymouth) is a project from Fedora and now listed among the [freedesktop.org's official resources](https://www.freedesktop.org/wiki/Software/#graphicsdriverswindowsystemsandsupportinglibraries) providing a flicker-free graphical boot process. It relies on [kernel mode setting](https://wiki.archlinux.org/index.php/Kernel_mode_setting) (KMS) to set the native resolution of the display as early as possible, then provides an eye-candy splash screen leading all the way up to the login manager.

### How to set it up?

**Download :** you can download via link below -
<p align="center">
  <a href="https://github.com/Mennaruuk/rocket-theme/releases/download/v1.0/rocket.zip"><img alt="undefined" src="https://img.shields.io/badge/Download-Here-orange?style=for-the-badge&logo=github"></a>
</p>

### How to use Rocket theme?

+ For **Debian** (Pop!_OS, Ubuntu, Kubuntu, etc.)-based distros:
```bash
# make sure you have the packages for plymouth
sudo apt install plymouth

# after downloading theme, copy the selected theme in plymouth theme dir
sudo cp -r rocket /usr/share/plymouth/themes/

# install the new theme
sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/rocket/rocket.plymouth 100

# select the theme to apply
sudo update-alternatives --config default.plymouth
#(select the number for installed theme, rocket in this case)

# update initramfs
sudo update-initramfs -u
``` 


### FYI
+ Thanks to @adi1090x! Rocket Theme is a fork of his [Plymouth Themes](https://github.com/adi1090x/plymouth-themes). Without his work, this wouldn't have been possible :) [Check out his page](https://github.com/adi1090x)! And his distro [Archcraft](https://archcraft-os.github.io/) :)
