Wake-On-Lan-Python
==================

wol.py is A small Python script to allow the sending of a WOL Magic packet so that LAN clients can be remotely switched on from another machine on the same subnet. Rather than needing to know the MAC address of the desired machine, the script allows you to specify by hostname, so long as that host is included in the configuration file.

I adapted this from an old version of [https://github.com/bentasker/Wake-On-Lan-Python](Wake-On-Lan-Python). You should probably use a new version of that instead of this repo.

Usage
-------

`wol.py [hostname]`

or

`wol.py list`


Configuration File
--------------------

The configuration file is a basic INI file, containing one section per host:

```
[General]
broadcast=192.168.1.255

[MyPc]
mac=00:13:0d:e4:60:61
```
