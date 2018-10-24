# <img max-height=10% src="https://www.chromium.org/_/rsrc/1438879449147/config/customLogo.gif?revision=3" alt="Chrome browser logo"> Encode Accelerator Implementation Status

This document shows the status of Chrome Media Recorder usage of hardware accelerated capabilities on the different platforms and hardwares. Updated **Feb 2018**.

Encoder   | Mac    | Android      | Windows     | Linux  | ChromeOs      |
--------- |:--:    | :-----:      | :-----:     | :----: | :------:      |
 H264     |&#10004;| &#10008; (1) | &#10004; (2)|&#10008;|  &#10004; (4) |
 VP8      |&#10008;| &#10004; (3) | &#10008;    |&#10008;|  &#10004; (4) |
 VP9      |&#10008;| &#10004; (3) | &#10008;    |&#10008;|  &#10008; (5) |

- (1) [crbug.com/719024](https://crbug.com/719024)
- (2) Available in Win8.1+ _and_ Cr &ge; 58.0.3023.0 ([crbug.com/590060](https://crbug.com/590060))
- (3) Cr &ge; M60.0.3088.0 ([crbug.com/638664](https://crbug.com/638664))
- (4) Cr &ge; M65.0.3324.0 on ARM devices only ([crbug.com/616659](https://crbug.com/616659)), not on Intel devices ([crbug.com/794608](https://crbug.com/794608)).
- (5) [crbug.com/811912](https://crbug.com/811912)

Support in Chrome for hardware accelerate encoding in Chrome OS depends on the actual chipset; the following table is

Chipset                           | H264     | VP8      | VP9      |
----------------------------------|:--------:|:--------:|:--------:|
Intel Atom (2014)                 | &#10004; |          |          |
Intel Broadwell (2014)            | &#10004; |          |          |
Intel Atom (2015)                 | &#10004; |          |          |
Intel Skylake (2015)              | &#10004; |          |          |
Intel Kabylake (2017)             | &#10004; | &#10004; | &#10004; |
Exynos 5250 (ARM)                 | &#10004; |          |          |
Exynos 5420/5800 (ARM)            | &#10004; | &#10004; |          |
Tegra T124/T132 (ARM)             | &#10004; | &#10004; |          |
Rockchip 3288 (ARM)               |          | &#10004; |          |
MediaTek 8173 (ARM)               | &#10004; | &#10004; |          |


