Yocto builds
============

To start a build on a build server for Nepos 1, run this:
```
$ repo init -u git@github.com:pascalhuerst/nonlinear-yocto -m yocto/manifests/default.xml
$ repo sync
$ mkdir -p ./build
$ source poky/oe-init-build-env `readlink -f ./build`
$ cp ../yocto/*.conf conf
$ bitbake nonlinear-image-default
```
