# raspi-z-buildtools

sudo apt-get install gawk wget git-core diffstat unzip texinfo gcc-multilib build-essential chrpath

repo init -u https://github.com/snst/raspi-z-baseline -b master

repo sync

. oe-init-build-env ../build

bitbake -e diet-image | grep "^DISTRO_FEATURES"

bitbake -e diet-image | grep "^MACHINE_FEATURES"
