#Network Scanner using Python

This Python script scans a network for active devices and retrieves their IP addresses, MAC addresses, and hostnames. It utilizes the scapy library for sending ARP packets and socket for resolving hostnames.

How It Works

    ARP Scanning:
    The script sends ARP (Address Resolution Protocol) requests to devices within a specified network range using scapy. It then listens for ARP replies to identify active devices.

    Threaded Scanning:
    To speed up the scanning process, the script uses multithreading. Each IP in the network range is scanned in a separate thread.

    Hostname Resolution:
    For each active device, the script attempts to resolve the hostname using socket.gethostbyaddr. If the hostname cannot be resolved, it defaults to "Unknown."

    Output:
    The results, including IP addresses, MAC addresses, and hostnames, are displayed in a well-formatted table.
