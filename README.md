# RTL8192EU
Linux driver for Realtek **RTL8192EU** based on official's **TP Link TL - WN823N V3 Beta** v5.2.19.1 from 2018-05-08 
<br>Supports monitor mode and frame injection for penetration testing abilities.

# Supported devices:
- DWA-131 _(untested)_
- GW-300S Katana _(untested)_
- TL-WN821N V6 _(untested)_
- TL-WN822N V5 _(untested)_
- TL-WN823N V3 _(tested)_

# Changelog:
- Added frame injection support
- Monitor mode is now supported
- Turned of powersaving
- Turned of debug
- Added compatibility for Linux Kernel v5.0-rc1
- Added compatibility for Linux Kernel v4.20
- Added compatibility for Linux Kernel v4.19+
- Added compatibility for Linux Kernel v4.15+

# Build guide

1. Make sure you have installed the following packages: 

```shell
    - make (Tested on 4.2.1)
    - gcc (Tested on 8.2.0)
    - git (OPTIONAL, Tested on 2.18.0)
    - libelf-dev
 ```

2. Download and unpack this repo, or just clone with git:

```shell
    $ git clone https://github.com/ZeeRooo/RTL8192EU.git
    $ cd RTL8192EU/
 ```
 
 3. Build the module:
 
 ```shell
    $ make clean
    $ make
    $ make install
 ```
 
  4. Load our shiny module:
 
 ```shell
    $ modprobe 8192eu
 ```
 
 # Original TP Link driver:
 https://static.tp-link.com/2018/201805/20180514/TP-Link_Driver_Linux_series8_beta.zip

