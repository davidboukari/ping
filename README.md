# ping

* Fix issue
```
$ sysctl -w net.ipv4.ping_group_range="0 1000"
sysctl: permission denied on key 'net.ipv4.ping_group_range'

$ sudo sysctl -w net.ipv4.ping_group_range="0 1000"
net.ipv4.ping_group_range = 0 1000

$ ping www.yahoo.fr
PING src.g03.yahoodns.net (212.82.100.150) 56(84) bytes of data.
64 bytes from w2.src.vip.ir2.yahoo.com (212.82.100.150): icmp_seq=1 ttl=50 time=30.1 ms
64 bytes from w2.src.vip.ir2.yahoo.com (212.82.100.150): icmp_seq=2 ttl=50 time=30.4 m
```
