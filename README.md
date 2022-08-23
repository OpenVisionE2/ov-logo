ov-bootvideo [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![ovboot](https://github.com/OpenVisionE2/ov-bootvideo/actions/workflows/ovboot.yml/badge.svg)](https://github.com/OpenVisionE2/ov-bootvideo/actions/workflows/ovboot.yml) [![ovbot](https://github.com/OpenVisionE2/ov-bootvideo/actions/workflows/ovbot.yml/badge.svg)](https://github.com/OpenVisionE2/ov-bootvideo/actions/workflows/ovbot.yml)
============
Bootvideo collection for Open Vision
* https://www.mp4compress.com is a good online tool for compress and make compatible h264 mp4

# bootlogo (Mipsel-SH4)

How to create 720p mvi bootlogo:
* ffmpeg -i bootlogo.jpg -r 25 -b 20000 -s hd720 bootlogo.m1v (type 1 - old)
* mv -f bootlogo.m1v bootlogo.mvi

# bootlogo (ARM)

How to create 1080p mvi bootlogo:
* ffmpeg -i bootlogo.jpg -r 25 -b:v 20000 -c:v mpeg2video -s hd1080 bootlogo.m1v (type 2 - new)
* mv -f bootlogo.m1v bootlogo.mvi

# HiSilicon splash

How to create 1080p img logo:
* ffmpeg -i logo.jpg -y -s 1920*1080 -pix_fmt yuvj420p logo.jpg
* python3 jpeg2hisi.py logo.jpg (https://github.com/OpenVisionE2/ov-bootvideo/blob/master/HisiLogoTool/jpeg2hisi.py)
