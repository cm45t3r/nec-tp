NEC Throughput
==============
Measures instant channel throughput by finding maximum packet size and computing sample average of raw ICMP requests of that size.

It uses a binary search algorithm to find maximum packet size, so it won't take more than a minute to finish.

Prerequisites
-------------
In order to run nec-tp smoothly, you must install [rawping](https://github.com/cm45t3r/rawping) first in your system. You must have root privileges to install and run.

Installing
----------
After cloning or copying the project, run `install` on a Unix shell from anywhere with root privileges.

Configuring
-----------
Edit `nectp` with your favorite editor and change lines below as your convenience. Default values was tested to work under nominal conditions.

```bash
# Configuration
PING_TIMEOUT=1
SAMPLE_SIZE=30
MAX_PACKET_SIZE=65535
```
Running
-------
On a Unix shell, run as it follows:

`nectp <host>`

- `host`: ip address or qualified hostname.
