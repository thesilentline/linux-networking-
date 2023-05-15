# Firewall

It is implementing a set of rules that govern access to a host that implements a web service for public access and an SSH service for administrative access. 

Iptables is still the default host firewall on many distributions, including our example Ubuntu distribution. Red Hat and CentOS v8 (on the Linux kernel 4.18), for instance, have nftables as their default firewall. The main reasons for moving to the new commands are to move toward a more consistent command set and provide better support of IPv6.

A firewall is a network security device that monitors incoming and outgoing network traffic and decides whether to allow or block specific traffic based on a defined set of security rules. Firewalls have been the first line of defense in network security for over 25 years.

## Why do we use firewall :

- Protects computer systems and networks from unauthorized access.
- Filters and monitors incoming and outgoing network traffic.
- Enforces security policies and access controls.
- Prevents unauthorized access to sensitive information.
- Reduces the attack surface of a network.
- Detects and blocks network-based attacks.
- Helps in intrusion prevention and detection.
- Provides application-level security by inspecting the content.
- Facilitates network segmentation and isolates network segments.
- Assists in compliance with industry and regulatory requirements.
- Plays a crucial role in overall network security.

## Features of Firewalls :

- **Logging and auditing**: Linux firewalls can log network traffic and firewall activity. Besides blocking unwanted traffic, this information can help monitor traffic patterns and identify unusual activity indicating a security breach. Firewall logs can also audit network activity to ensure compliance with company policies and procedures. Thus, organizations can leverage Linux firewall logging capabilities to gain valuable insights into their network traffic and proactively maintain security and system integrity.
- **Packet filtering**: Linux firewalls secure your network by examining both incoming and outgoing packets. They can be customized to block traffic that does not meet your predefined criteria, such as specific IP addresses, ports, or protocols. Reliable firewalls are more important than ever for ensuring your network remains safe and secure.
- **Network Address Translation (NAT)**: Linux firewalls can perform NAT, which allows multiple devices to share a single public IP address while keeping internal IP addresses hidden from the internet. This is particularly useful in scenarios where multiple users need to access the internet simultaneously, as it can help distribute bandwidth more evenly. Additionally, firewalls can perform other functions such as packet filtering, intrusion detection, and VPN connectivity. By using a firewall, users can ensure that their network is secure and that their data is protected from malicious attacks.
- **Stateful packet inspection**: Linux firewalls are crucial for network security, as they perform stateful packet inspection to track and distinguish between legitimate and illegitimate traffic. This feature effectively blocks any unwanted access to the network. They are also highly customizable, allowing network administrators to set up VPNs, define rules for specific types of traffic, and more. Overall, Linux firewalls are a vital component of a comprehensive network security strategy to protect against unauthorized access and security threats.
- **Application layer filtering**: Linux firewalls can filter traffic based on application-level data, such as HTTP headers or email messages, to prevent attacks that exploit vulnerabilities in specific applications. By filtering out malicious traffic before it reaches the application layer, Linux firewalls improve network security.

## How are all the features in the firewall implemented:

- A firewall may be implemented as a hardware device (such as a Linksys or Netgear firewall you can buy in an electronics store) or in software, such as the Windows Firewall or the MacOS Firewall. Unix and Linux users may be familiar with the iptables firewall.
- Netfilter: Netfilter is a tool inside Linux that lets you create your own ways of handling different types of networking tasks.
- iptables: iptables is a powerful tool that lets you control how data moves through your computer's firewall. You can use it to manage network traffic in many ways, and it's easy to learn.
- nftables: nftables is part of the Linux kernel and helps filter and organize network data like packets and frames.
- Nftables is a subsystem within the Linux kernel that allows for the filtering and organization of network data such as packets, datagrams, and frames. It is a newer and more customizable alternative to iptables, the default firewall on many Linux distributions, including Ubuntu. Red Hat and CentOS v8 have nftables as their default firewall. Nftables provides a more consistent command set and better support for IPv6. It is an important component of network security, helping to protect against unauthorized access and security threats.
- Uncomplicated Firewall (UFW): UFW is a program that makes it easy to manage firewalls on Linux systems. It uses simple commands and works with iptables for configuration.
- Firewalld: Firewalld helps you restrict access to services, ports, and networks. You can use it to block specific subnets and IP addresses. Like other firewalls, it checks all traffic going through the system's interfaces.
- Shorewall: Shorewall is a tool that helps you manage gateways and firewalls on GNU/Linux systems. It makes it easier to set up iptables rules by using a simpler, more user-friendly configuration file format that's easier to read and understand.

**Actual Time Taken 5hrs**