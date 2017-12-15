Yocto builds
============

To create an image for nonlinear embedded devices, run this:
```
$ repo init -u git@github.com:pascalhuerst/nonlinear-yocto -m yocto/manifests/default.xml
$ repo sync
$ mkdir -p ./build
$ source poky/oe-init-build-env `readlink -f ./build`
$ cp ../yocto/*.conf conf
$ bitbake nonlinear-image-default
```
