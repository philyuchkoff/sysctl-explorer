---
layout: sysctl
title: udp_wmem_min
sysctl-category: net.ipv4
sysctl-file: /proc/sys/net/ipv4/udp_wmem_min
sysctl-variable: net.ipv4.udp_wmem_min
source: https://www.kernel.org/doc/Documentation/networking/ip-sysctl.txt
---
Minimal size of send buffer used by UDP sockets in moderation.
Each UDP socket is able to use the size for sending data, even if
total pages of UDP sockets exceed udp_mem pressure. The unit is byte.
Default: 1 page

