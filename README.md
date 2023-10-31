# openbikegps-project

## Quick start

To build the Yocto image using KAS use the command
```
kas build kas/board/raspberrypi4.yml:kas/image/core-image.yml
```
You can of course use another image from the kas/image folder according to your device.

## Setup

To be able to build the image you need to install at least the [build host packages](https://docs.yoctoproject.org/brief-yoctoprojectqs/index.html#build-host-packages) and [KAS](https://github.com/siemens/kas)

Build host packages:
```
sudo apt install gawk wget git diffstat unzip texinfo gcc build-essential chrpath socat cpio python3 python3-pip python3-pexpect xz-utils debianutils iputils-ping python3-git python3-jinja2 libegl1-mesa libsdl1.2-dev python3-subunit mesa-common-dev zstd liblz4-tool file locales
sudo locale-gen en_US.UTF-8
```

KAS:
```
sudo apt install kas
```
