RetroPie for the Rock64 RK3328
==============

Tested On Ubuntu
-------------

This fork of RetroPie-Setup has been tweaked to bypass the unknown architecture error for this device:
https://roc-rk3328-cc.readthedocs.io/en/latest/intro.html#specification

This build was tested and run on Ubuntu 16.04 
```shell
sudo apt-get update
sudo apt-get dist-upgrade
sudo apt-get install git
```

Then you can download the latest RetroPie setup script with

```shell
cd
git clone --depth=1 https://github.com/MattAndrzejczuk/RetroPie-Setup-for-ROCK64-PINE64.git
```

The script is executed with 

```shell
cd RetroPie-Setup-for-ROCK64-PINE64
sudo ./retropie_setup.sh
```

Thanks
------

This fork of the original script simply tells the installer that you're running on an ODROID-C2 board which has a similar ARM Cortex-A53
