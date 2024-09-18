---
draft: true
title: "ciBPF"
date: 2024-09-18T00:00:00+08:00
---

# Under construction

## CibouletteBPF

CibouletteBPF aka ciBPF is a red team evasion tool based on eBPF developped in C. In this post we will explain how it works and its use-cases

### Context

During a red team exercice, we can be facing a computer located in a DMZ or in any other segmented area. If this computer has any open port, for example a webserver on p.443, eBPF could help us to "hijack" this connection and send information and trigger the program.

### eBPF program

Let's start with the explanation of our program in details

#### Network sniffing

Ok so the first thing our program needs to do is listen to a network interface on the victim's computer in order to receive the packets from the attacker. For that we will use the XDP, which is a technology avaible from eBPF to listen and manage network packets. We will also have to hook our program to a network interface (here enp0s3).

####  Extraction of needed information

#### Stock in map

### Loading & executing

either a loader or bpftools: 
1. Map creation
2. Loading
3. attaching

#### Loading the program in the linux kernel

#### Retrieving information in the map

#### Executing the command in the userspace

#### Getting the output

### Testing part

Now that our programs are ready, let's test them in a dev environement

#### Custom network protocol 

In order to test it in dev mode, we made a custom network protocol over TCP. ...

#### Results and interpretation

### Conclusion
