# raspi-z-buildtools

sudo apt-get install gawk wget git-core diffstat unzip texinfo gcc-multilib build-essential chrpath


. oe-init-build-env ../build

bitbake -e diet-image | grep "^DISTRO_FEATURES"

bitbake -e diet-image | grep "^MACHINE_FEATURES"
