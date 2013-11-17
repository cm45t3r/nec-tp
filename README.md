NEC Throughput
==============
Measures instant channel throughput by finding maximum packet size and computing sample average of raw ICMP requests of that size.

It uses a binary search algorithm to find maximum packet size, so it won't take more than a couple of minutes to finish.

Prerequisites
-------------
In order to run nec-tp smoothly, you must install [rawping](https://github.com/cm45t3r/rawping) first in your system. You must have root privileges to install and run.

Installing
----------
Copy or clone the project:
```bash
git clone https://github.com/cm45t3r/nec-tp.git
```
Run `./install` as root on a Unix shell and that's is.

Configuring
-----------
Whether you are interested on customizing <b>nectp</b> to improve performance or accuracy, go and edit `/usr/bin/nectp` in your favorite editor with root privileges and change lines below as your convenience. Default values was tested to work under nominal conditions for general purpose.

```bash
# Configuration
PING_COUNT=1
PING_TIMEOUT=1
SAMPLE_SIZE=30
MAX_PACKET_SIZE=65500
```
Running
-------
On a Unix shell, run as it follows:

`nectp <host>`

- `host`: ip address or qualified hostname.
