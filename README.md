NEC Throughput
==============

Installing
----------
In order to run nec-tp smoothly, you must install [rawping](https://github.com/cm45t3r/rawping) first.

Configuring
-----------
To setup nec-tp open `nec-tp` in an editor and modify the following parameters (we show default values):

```bash
PING_TIMEOUT=1
SAMPLE_SIZE=30
MAX_PACKET_SIZE=65535
```

Usage
-----
As a bash app, call from bash shell:

`nectp <host>`

Where host is an IPv4 address or qualified hostname.
