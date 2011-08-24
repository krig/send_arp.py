# send_arp.py

A python implementation of send_arp.c.

Uses no code from the original, depends only on standard python modules.

Run as root, uses raw sockets.

ARP code and license inspired by arprequest by Antoine Millet.

See http://pypi.python.org/pypi/arprequest

# Usage

    send_arp.py [-i interval(ms)] [-r repeat] [-p pidfile] \
        device src_ip src_mac broadcast netmask
    
* PID file is always ignored.

* Netmask is always ignored.
    
This code sends two ARP packets per interval to maximize
likelihood of not being filtered.

# License

    /* This program is free software. It comes without any warranty, to
     * the extent permitted by applicable law. You can redistribute it
     * and/or modify it under the terms of the Do What The Fuck You Want
     * To Public License, Version 2, as published by Sam Hocevar. See
     * http://sam.zoy.org/wtfpl/COPYING for more details. */
