# pyrestore
[![Packagist](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org)<br>
Simple tool to prepare a modified IPSW for idevicererestore working with [Alitek's](https://twitter.com/alitek123) bug

### Usage

`usage : ./pyrestore.py -i <ipsw_in> <ipsw_out> -m <build_manifest> -b <baseband>`

You need : 
 - **BuildManifest.plist** you correctly patched
 - **Baseband** from the latest signed IPSW for your device 
 - **IPSW** you want to downgrade to <br>

Make sure to have all the files in the same directory. Then run pyrestore as followed : <br>
`./pyrestore.py -i iPhone5,4_9.3.2_13F69_Restore.ipsw custom.ipsw -m BuildManifest.plist -b Mav7Mav8-7.21.00.Release.bbfw` <br>
Default baseband in the IPSW is not removed, because it is not needed <br>
Also, if a directory named "IPSW" already exists, it will be removed <br>

### Installation 
If you want to install it, copy pyrestore to your `$PATH`. eg : `sudo cp pyrestore.py /usr/local/bin`

### Credits 

Everything goes to the [downgrade.party](https://downgrade.party) team <br>
Script written by [matteyeux](https://twitter.com/matteyeux) <br>

Here is a [quick demo of idevicererestore running under VMware](https://www.youtube.com/watch?v=1Gfb1k-hpCk)
