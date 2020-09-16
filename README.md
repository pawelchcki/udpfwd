## udpfwd

udpfwd forwards UDP packets from a specified incoming address to an outgoing address.

```
usage: udpfwd --in host:port --out host:port
```

udpfwd also emits the following metrics to the outgoing host:port:

* `udpfwd.in_bytes` bytes read from incoming address
* `udpfwd.out_bytes` bytes read from outgoing address
* `udpfwd.error` number of errors encountered (tagged by "direction:{in,out}")
