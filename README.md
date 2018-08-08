# RTL8192EU
Linux driver for Realtek **RTL8192EU** based on official's **TP Link TL - WN823N V3 Beta** driver from 2018-05-08 

# Supported devices:
- TL-WN821N V6 _(untested)_
- TL-WN822N V5 _(untested)_
- TL-WN823N V3 _(tested)_

# Changelog:
- Added compatibility for Linux Kernel 4.15+

# Build guide

1. Make sure you have installed the following packages: 

```shell
    - make (Tested on 4.2.1)
    - gcc (Testedr on 8.2.0)
    - git (OPTIONAL, Tested on 2.18.0)
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
    # make install
 ```
 
  4. Load our shiny module:
 
 ```shell
    # modprobe 8192eu
 ```
 
 # Original TP Link driver:
 https://static.tp-link.com/2018/201805/20180514/TP-Link_Driver_Linux_series8_beta.zip

