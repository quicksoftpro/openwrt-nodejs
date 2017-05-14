OpenWrt package feed for nodejs
=====

[![Build Status](https://travis-ci.org/quicksoftpro/openwrt-nodejs.svg?branch=master)](https://travis-ci.org/quicksoftpro/openwrt-nodejs)

This is an OpenWrt package feed containing community maintained nodejs packages.

This is a fork from https://github.com/xinpascal/openwrt-nodejs

we have changed the version of nodejs oto 7.x

To use these packages, add the following line to the feeds.conf
in the OpenWrt buildroot:

	src-git nodejs git://github.com/quicksoftpro/openwrt-nodejs.git
  
Update the feed:

	./scripts/feeds update nodejs 
  
Activate the package:

	./scripts/feeds install -a -p nodejs
  
The nodejs packages should now appear in menuconfig.


