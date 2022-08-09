ov-bootvideo [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![ovboot](https://github.com/OpenVisionE2/ov-bootvideo/actions/workflows/ovboot.yml/badge.svg)](https://github.com/OpenVisionE2/ov-bootvideo/actions/workflows/ovboot.yml) [![ovbot](https://github.com/OpenVisionE2/ov-bootvideo/actions/workflows/ovbot.yml/badge.svg)](https://github.com/OpenVisionE2/ov-bootvideo/actions/workflows/ovbot.yml)
============
Bootvideo collection for Open Vision
* https://www.mp4compress.com is a good online tool for compress and make compatible h264 mp4

# bootlogo

How to create 720p mvi bootlogo:
* ffmpeg -i bootlogo.jpg -r 25 -b 20000 -s hd720 bootlogo.m1v
* mv -f bootlogo.m1v bootlogo.mvi
