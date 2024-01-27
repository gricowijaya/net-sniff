# Script Explanation

This script will analyze the wireless interface of your computer to sniff your network traffic the script will identify the wireless interface using `iwconfig`

# How to use this script 

make the `sniff` script to be executable using 

```bash
chmod -x sniff
```

Pass the flag of:

- `-t` for providing the seconds of time such as `-t 10` for 10 seconds or `-t 100` for 100 seconds 
- `-o` name for the output file it will generate a `.pcap` for the network traffice, `.txt` for the list of packet, and `.details.txt` for the details of the packet

example: 

```bash
./sniff -t 10 -o my-network-traffic
```

## Demo Video

~[demo](./demo/video.mp4)

# Analyzying the Network Traffic

Analyzing a `.pcap` file can reveal a lot of information about network traffic. Here are some areas you might want to focus on:

1. **Network Devices**: By analyzing the MAC addresses and IP addresses in the `.pcap` file, you can identify the devices on your network. This includes computers, printers, routers, etc. [Source 2](https://apackets.com/).

2. **Protocols**: The `.pcap` file contains data for various network protocols. You can analyze the data for specific protocols to understand how they are being used. For example, you can analyze HTTP requests and responses, DNS queries and responses, etc. [Source 2](https://apackets.com/).

3. **Traffic Patterns**: By examining the timestamps and sizes of the packets, you can get an idea of the network's traffic patterns. For example, you might notice spikes in traffic at certain times, or certain types of traffic occurring more frequently.

4. **Security Issues**: If you're interested in network security, you might look for signs of malicious activity. This could include unusual traffic patterns, attempts to exploit known vulnerabilities, etc. [Source 2](https://apackets.com/).

5. **Performance Issues**: By analyzing the `.pcap` file, you can identify potential performance issues. For example, you might notice high latency, packet loss, or other problems that could affect network performance.

Remember, the specific things you need to analyze will depend on why you're capturing the network traffic. If you're trying to troubleshoot a problem, you might focus on the specific protocols and devices involved. If you're trying to optimize network performance, you might look for general trends in traffic patterns and performance metrics.
