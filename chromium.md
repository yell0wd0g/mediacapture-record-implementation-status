# <img max-height=10% src="https://www.chromium.org/_/rsrc/1438879449147/config/customLogo.gif?revision=3" alt="Chrome browser logo"> Encode Accelerator Implementation Status

This document shows the status of Chrome Media Recorder usage of hardware accelerated capabilities on the different platforms and hardwares. Updated **January 2017**.

Encoder   | Mac| Android                  | Windows | Linux | ChromeOs |
--------- |:--:| :-----:                  | :-----: | :----:| :------: |
 H264     |&#10004; | [crbug.com/638664](https://crbug.com/638664) | &#8805; 58.0.3023.0 (1) |&#10008;|  [crbug.com/616659](https://crbug.com/616659) |
 VP8      |&#10008;| [crbug.com/638664](https://crbug.com/638664) |&#10008;|&#10008;|  [crbug.com/616659](https://crbug.com/616659) |

(1) Available in Win8.1+ ([crbug.com/590060](https://crbug.com/590060))

At the time of writing, VP9 hardware encode acceleration is supported in no platforms.

Support in Chrome for hardware accelerate encoding in Chrome OS depends on the actual chipset; the following table is

Chipset                           | H264     | VP8      |
----------------------------------|:--------:|:--------:|
Intel Atom (2014)                 | &#10004; |          |
Intel Broadwell (2014)            | &#10004; |          |
Intel Atom (2015)                 | &#10004; |          |
Intel Skylake (2015)              | &#10004; |          |
Exynos 5250 (ARM)                 | &#10004; |          |
Exynos 5420/5800 (ARM)            | &#10004; | &#10004; |
Tegra T124/T132 (ARM)             | &#10004; | &#10004; |
Rockchip 3288 (ARM)               |          | &#10004; |
MediaTek 8173 (ARM)               | &#10004; | &#10004; |


