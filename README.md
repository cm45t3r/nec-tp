NEC Throughput
==============

Pre-requisites
-------------
In order to run nec-tp smoothly, you must install [rawping](https://github.com/cm45t3r/rawping) first.

Installing
----------
After cloning or copying the project, run `install` on a Unix shell from anywhere with root privileges.

COnfiguring
-----------
Edit `nec-tp` using your favorite text editor and change lines below as your convenience. Default values are tested to work under nominal conditions:

```bash
PING_TIMEOUT=1
SAMPLE_SIZE=30
MAX_PACKET_SIZE=65535
```

Running
-------
Just run on a Unix shell as it follows:

`nectp <host>`

- `host`: ip address or qualified hostname.
