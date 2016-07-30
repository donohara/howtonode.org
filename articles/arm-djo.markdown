Title: Fun Putting xxxx  Node on Mobile Devices
Author: wwwww dddddd 
Date: Fri Jul 01 2011 10:04:02 GMT-0700 (PDT)
Node: v0.4.9

This article will walk you through creating an Ubuntu image that can be chrooted inside a mobile device like the recently released [TouchPad][].  Once the Ubuntu environment is setup we'll learn how to compile and install node for fun and/or profit.

## Create the Image

hen log into the device and mount it on the internal drive.

    novaterm
    mkdir /media/chroot
    mount /media/internal/UbuntuNatty_armel.img /media/chroot
    mount -t proc none /media/chroot/proc
    mount -t sysfs none /media/chroot/sys
    mount -o bind /dev /media/chroot/dev
    cp /etc/resolv.conf /media/chroot/etc/resolv.conf

