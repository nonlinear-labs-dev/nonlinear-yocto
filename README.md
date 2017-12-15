# Extreeme Quickstart

mkdir -p ./build
source poky/oe-init-build-env `readlink -f ./build`
cp ../yocto/*.conf conf
bitbake nonlinear-image-default
