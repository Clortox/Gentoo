# Gentoo
Welcome! 

This repo will house everything needed to copy my personal build of Gentoo I use on my system. Ideally you should tweak this to your own preferences, and change things according to your hardware. 

I can't guarentee that this build is the best possible version of my kernel for my hardware, however it works well enough and is lighter and faster than any other OS I've put onto my system.

## Laptop Specs
  - OMEN by HP Laptop 15-dc1xxx
  - Intel i7-9750H (12 core) @ 4.5Ghz
  - NVIDIA GeForce GTX 1660 Ti Mobile
  - 16 GB Memory, 256 GB NVMe, 1TB HDD
  
This is the base system; I have not modified it in any way.

## Kernel
  - Gentoo Hardened Kernel 5.9.12
  - Hardened Stage3 Package
  - NETFS support (smba)
  - SDR Support (HackRf)
  - Works with built in LEDs, Camera, Microphone, Integrated/Dedicated GPU, Fans, ACPI, Touchpad Gestures, and WiFi
  
Please refer to /kernel for my .config to build the system using emerge

## Enviroment
  - X11
  - dwm
    - Gaps
  - st
    - Scrolling
    - Alpha
  - dmenu
  - slock
  
Copies of all of these can be found in /desktopenv

My DWM also has custom keybindings to make it easier to manuvere across my 3 screen setup.

## Portage
  A copy of my make.conf can be found in /portage

## Quirks
  NVIDIA Drivers took a bit of trial and error for me to setup. I chose to use the propieritary drivers included in x11-drivers/nvidia-drivers. This took a couple of trys, however if you choose to use my .config you shouldn't have any issues after emerging that package. 
  
  Audio was difficult to setup at first, however the drivers should be enabled in my .config to work out of the box. I use commandline pulse tools to manage my audio, such as media-sound/pulsemixer.
 
 Steam can be quite finicky, however when using the ebuild imported via layman it seems to work very well, and proton runs perfectly.
 
## Other Software
  - [Firefox](https://packages.gentoo.org/packages/www-client/firefox-bin)
  - [Discord](https://discord.com/download) (Dont use emerge, the tar.gz works better)
  - [ncspot](https://github.com/hrkfdn/ncspot) (Spotify)
  - [apvlv](https://packages.gentoo.org/packages/app-text/apvlv) (Pdf/Epub reader)
  - [vim](https://packages.gentoo.org/packages/app-editors/vim) (Text editor)
  - [cronie](https://packages.gentoo.org/packages/sys-process/cronie) (Cron daemon)
  - [hackrf-tools](https://packages.gentoo.org/packages/net-wireless/hackrf-tools) (Work with SDR)
  - [wpa_supplicant](https://packages.gentoo.org/packages/net-wireless/wpa_supplicant) (Cli Wifi)
  - [Gimp](https://packages.gentoo.org/packages/media-gfx/gimp) (Image manipulation)
  - [Slic3r](https://github.com/slic3r/Slic3r/wiki/Running-Slic3r-from-git-on-GNU-Linux#gentoo) (3D Printing)
  - [Blender](https://packages.gentoo.org/packages/media-gfx/blender) (Modeling)
  - [feh](https://packages.gentoo.org/packages/media-gfx/feh) (view images)
  - [vlc](https://packages.gentoo.org/packages/media-video/vlc) (video viewer)
  - [bash](https://packages.gentoo.org/packages/app-shells/bash) (shell)
  - [tmux](https://packages.gentoo.org/packages/app-misc/tmux) (terminal multiplexer)
