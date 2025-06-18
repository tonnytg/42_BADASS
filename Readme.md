# Badass (BGP At Doors of Autonomous System is Simple)

### Introduction

The purpose of this project is to expand the knowledge you have gained through NetPractice. You will have to simulate a network and configure it using GNS3 with docker images.
BGP EVPN is based on BGP (RFC 4271) and its extensions, MP-BGP (RFC 4760).
BGP is the routing protocol that drives the Internet. Through MP-BGP extensions, it
can be used to carry reachability information (NLRI) for various protocols (IPv4, IPv6, L3
VPN and in this case, EVPN). EVPN is a special family used for publishing information
about MAC addresses and the end devices that access them.


### Instruction

- Virtual Machines
- Install Docker and GNS3
- You have to put all the configuration files of your project in folders located at
the root of your repository (see section “Submission and peer-evaluation” for more
information). The folders of the mandatory part will be named: P1, P2 and P3.


# Mandatory

This project involves setting up several environments under specific rules.
It is divided into three parts you have to do in the following order:
• Part 1: GNS3 configuration with Docker.
• Part 2: Discovering a VXLAN.
• Part 3: Discovering BGP with EVPN.

# P1

- Install Docker and GNS3
- Create one image using Alpine but with no extra packages
- Create another image using Alpine but with extra packages bgp, vxlan, etc...
- Open GNS GUI and add new Docker Compute and apoint to Image One and Image Two
- Now you have two computers simulating a simple network
