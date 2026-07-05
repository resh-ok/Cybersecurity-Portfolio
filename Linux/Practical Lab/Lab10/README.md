# Lab 10: Basic Networking Commands

## Objective

The objective of this lab is to learn how to inspect basic network configuration and test network connectivity using essential Linux networking commands. These commands are widely used in system administration, troubleshooting, and cybersecurity investigations.

## Learning Outcomes

By completing this lab, I learned how to:

* View network interface information.
* Display the system's IP address.
* View the routing table.
* Test network connectivity.
* Display active network connections and listening ports.

## Commands Used

### Display Network Interfaces

```bash id="9eq0fi"
ip addr
```

Displays information about all network interfaces, including IP addresses and interface status.

---

### Display the Routing Table

```bash id="94fh61"
ip route
```

Displays the system's routing table and default gateway.

---

### Test Network Connectivity

```bash id="h87op2"
ping google.com
```

Sends ICMP echo requests to test connectivity with a remote host.

Press **Ctrl + C** to stop the command.

---

### Display Active Network Connections

```bash id="gndiqw"
ss -tuln
```

Displays listening TCP and UDP ports without resolving hostnames.

**Options:**

* `-t` – TCP sockets
* `-u` – UDP sockets
* `-l` – Listening sockets
* `-n` – Display numeric addresses and port numbers

## Observations

* The `ip addr` command displayed the available network interfaces and their assigned IP addresses.
* The `ip route` command showed the default gateway and routing information.
* The `ping` command successfully tested communication with a remote host.
* The `ss -tuln` command displayed active listening ports and network services.

## Security Insight

Network commands are essential tools for cybersecurity professionals. Analysts use them to verify network connectivity, identify IP addresses, inspect routing information, and detect services listening on network ports. Reviewing listening ports is particularly useful when identifying unauthorized or unnecessary network services that could increase a system's attack surface.

## Summary

This lab introduced essential Linux networking commands used to inspect network configuration and troubleshoot connectivity. Understanding how to view network interfaces, routing information, and listening ports provides a strong foundation for network administration and cybersecurity analysis.
