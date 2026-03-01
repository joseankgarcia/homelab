# Hardware Overview

## Primary Server
#### Hardware Specifications
- CPU: Intel XEON E5-2620 v3
- Memory: 128GB DDR4 ECC
- Boot Drive: 1TB Crucial P3 Plus NVMe
- Storage: 2 x 4TB Western Digital Red Plus (Mirror VDev)
- Chassis: 3U Rackmount Server

#### Primary Workloads
- Proxmox Hypervisor
- TrueNAS Data Platform 
- Zero-Trust Network Access
- Reverse Proxy
- Monitoring & Logging
- Backup DNS
- Media Services
- Automation & Data Processing


## Secondary Server
#### Hardware Specifications 
- CPU: H616 64-Bit
- Memory: 512MB
- Boot Drive: 16GB MicroSD
- Storage: Primary Server

#### Primary Workloads
- DNS Server
- PiHole DNS Sinkhole
- DNS Dashboard

## Networking Infrastructure
#### Router
- MikroTik hEX S

#### Switching
- NETGEAR 8-Port Gigabit Smart Switch
- VLAN-Capable segmentation

#### Wireless (WAN)
- TP-Link EAP610 Access Point
- Dedicated VLAN for wireless clients

## Physical Infrastructure
- TRENDnet 24-Port Patch Panel
- CAT-6 RJ-45 Cabling
- Server Rack 



### Power consumption values are estimated using hardware TDP and expected utilization.
-  Estimated Average: ~150w
-   Estimated Peak: ~250w
