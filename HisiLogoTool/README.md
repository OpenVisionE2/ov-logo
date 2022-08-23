HisiLogoTool [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![ovboot](https://github.com/OpenVisionE2/ov-bootvideo/actions/workflows/ovboot.yml/badge.svg)](https://github.com/OpenVisionE2/ov-bootvideo/actions/workflows/ovboot.yml) [![ovbot](https://github.com/OpenVisionE2/ov-bootvideo/actions/workflows/ovbot.yml/badge.svg)](https://github.com/OpenVisionE2/ov-bootvideo/actions/workflows/ovbot.yml)
============
Lost the boot logo and want it back?

First upload (FTP) logo.img into /tmp then use telnet/ssh: 
* dd if=/tmp/logo.img of=/dev/block/by-name/logo 

To save original logo.img use:
* dd if=/dev/block/by-name/logo of=/tmp/logo.img 

To strip the dumped file:
* strip.py logo.img 

To convert the extracted logo to jpeg:
* hisi2jpeg.py logo.img 

To convert your own jpeg logo to HiSilicon format:
* ffmpeg -i logo.jpg -y -s 1920*1080 -pix_fmt yuvj420p logo.jpg
* jpeg2hisi.py logo.jpg
