# mcast-quick-demo

## Example iPerf Multicast Commands for Linux Hosts

### Sender

```bash
iperf -c 239.0.30.101 -u -b 10pps -T 100 -t 3600 -i 1
```

### Receiver ASM Join (*,G)

```
iperf -s -u -B 239.0.30.101 -i 1
```

### Receiver SSM Join (S,G)

```bash
iperf -s -u -B 239.0.30.101 --ssm-host 10.30.30.103 -i 1
```

**Modify multicast groups as needed for testing**