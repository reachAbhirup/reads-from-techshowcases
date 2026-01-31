---
title: "Understanding Network Devices"
seoTitle: "Guide to Network Devices"
datePublished: Sat Jan 31 2026 13:14:09 GMT+0000 (Coordinated Universal Time)
cuid: cml2c2mfp000402kz2mti1txy
slug: understanding-network-devices
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1769167790420/3128df3c-0e89-4977-8ac6-78786d96a3a2.png
tags: networking, computer-networking, chaiaurcode, chaicode, chaicohort, chai-code, chaicode-webdev-cohort-2026, dns-networkingbasics-internetbasics-webfundamentals-computernetworks-techforbeginners-learnnetworking-webdevelopment-howinternetworks-csbasics

---

In 2026, where hardly any device is not connected to internet, it is quite confusing and messy to understand what constitutes to computer network and which devices or hardwares are fundamentally responsible for successful communication between world wide web of computers. When I was in my college days, my teachers suggested me to understand this inter computer network of WWW as if, it is a layout of water pipeline plan for a very big city (at today’s scale, probably we need to visualize the whole world as one big city). The data that flows through internet, is the waterflow, and network devices are the “plumbers“ who ensures that water flows from intended source to intended target, following an approach of finding least distance path, to reach the target without any delay.

Hello! My name is Abhirup Roy, I build softwares and I write about them. Though we engineers have a special fond for fancy technical terms, I prefer simplicity over jargons. Let’s dive back to our Computer Networks 101 and understand essential network devices in a `TL;DR` fashion with real-life examples and easy to visualize analogies.

Today’s computer network, is built on a design strategy where a computer network has been segregated in groups, in such a way, that our data flow is contained within these groups. Bigger the geographical area the network covers, more iteration of this design, resulting in multiple copies of these network groups. These groups are -

* WWW User Devices
    
* Local Network
    
* Enterprise Network
    
* ISP Edge
    
* Internet Backbone
    
* Datacenter
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1769168166093/a58c25ee-f91b-496c-88b1-a3d501174e7c.png align="center")

Each of these groups have their respective role in establishing and maintaining data flow, and in order to do that, each of these groups use few network devices. Thus these are the most common and will be part of this discussion. Remember, internet is an ongoing evolution from ARPANET project in **1969,** to transition to official internet with standard TCP/IP protocol allowing different networks to connect, happened on January 1, 1983, and each component used in internet has its scope of diving very deep (from hardware implementation to software abstraction of each network device used). But in this article, my objective is to explain network device and how they make computer network work, without getting into “rabbit hole”, hence `TL;DR` approach.

Before I explain the above network architecture, first I want to talk about another concept, that we need to refer to in our journey to understand computer networking. Open Systems Interconnection AKA OSI model. It is a conceptual framework that segregate/standardize network communication functions/operations into manageable stages (🤯😵‍💫).

Basically it is a 7-stage layered approach in which computer network communication happens. So, at each layer, which ever networking function is performed, its relevant hardwares and few rules that these hardwares follow to operate, are involved. I have prepared a diagram to show you that at each of 7 layers of OSI framework, certain network functions are performed by respective hardwares, using respective protocols (in simple term, rules).

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1769186680589/1b51e602-4fde-46d6-b0f8-9e44c0aa5c69.png align="center")

* Physical layer AKA Layer 1 handles raw electrical and optical signals. Hence devices that works at this layers not “intelligent” enough to understand IP address and MAC addresses. Hence, they take incoming electrical signals and send them out to all devices after performing its duties. In this layer we have below devices -
    
    1. Hub - A central connection point for devices in a LAN. It takes an incoming signal on one port and blindly broadcasts it to all other ports. This leads to collisions when multiple devices try to talk at once, reducing efficiency and security risks (everyone sees everyone's data). Preferably, in real-life, hubs are avoided as switch is a better alternative.
        
    2. Repeaters - A repeater is a network device that regenerates weakened or corrupted signals to restore them to their original form before re-transmission. Unlike an amplifier, which increases both signal and noise, a repeater reconstructs the original clean signal and forwards it, ensuring reliable data delivery over longer distances.
        
    3. Modem - Is an abbreviation of two words - Modulator and Demodulator.