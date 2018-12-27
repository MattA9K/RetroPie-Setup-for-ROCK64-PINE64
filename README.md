RetroPie for the Rock64 RK3328
==============

Tested On Ubuntu
-------------

This fork of RetroPie-Setup has been tweaked to bypass the unknown architecture error for this device:
https://roc-rk3328-cc.readthedocs.io/en/latest/intro.html#specification


Start just like you do with the official git repo:

```shell
cd
git clone --depth=1 https://github.com/MattAndrzejczuk/RetroPie-Setup-for-ROCK64-PINE64.git
```

Haven't figured this out yet whether you need to do this before or after installation, but these packages are required in order to get emulationstation working:

```shell
sudo apt-get install libsdl2-dev
sudo apt-get install libudev-dev
sudo apt-get install libibus-1.0-dev
sudo apt-get install fcitx-libs-dev
```


Give it a shot, run the installer:

```shell
cd RetroPie-Setup-for-ROCK64-PINE64
sudo ./retropie_setup.sh
```

Thanks
------

This fork of the original script simply tells the installer that you're running on an ODROID-C2 board which has a similar ARM Cortex-A53 architecture.
