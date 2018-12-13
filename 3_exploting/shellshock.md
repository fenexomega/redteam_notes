https://github.com/fenexomega/icmpshock

For Receiving ping connections:

tcpdump -nni any -e "icmp[icmptype] == 8"
