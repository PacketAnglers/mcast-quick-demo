# mcast-quick-demo

## Example iPerf Multicast Commands for Linux Hosts

### Sender

```bash
iperf -c 239.0.30.101 -u -b 10pps -T 100 -t 3600 -i 1
```

### Receiver

```
iperf -s -u -B 239.0.30.101 -i 1
```

Replace multicast groups as needed