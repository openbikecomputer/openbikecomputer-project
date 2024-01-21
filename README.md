# openbikegps-project

## Quick start

Build the Yocto image using KAS use the command
### Raspberry-Pi 4 (dev only)
```
kas build kas/board/raspberrypi4.yml:kas/image/core-image.yml
```

### Bryton Rider 860
```
kas build kas/board/brytonrider860.yml:kas/image/core-image.yml
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

## Install and use KAS in python virtual-env (venv)

### Create the venv and install KAS in it
```
python3 -m venv .venv
source .venv/bin/activate
python3 -m pip install --upgrade pip
python3 -m pip install kas
```

### Activate the venv
```
source .venv/bin/activate
```

### Deactivate the venv
```
deactivate
```
