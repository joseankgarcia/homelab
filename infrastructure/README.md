# Infrastructure Overview

This infrastructure overview defines the rack layout, hardware specifications, storage, and VLAN design components of the homelab.

The homelab’s primary server is managed through Proxmox, which is the virtual environment host for other hosts on the bare metal proxmox machine. This houses my storage architecture (TrueNAS) and Docker containers (Debian). The other secondary server is managed using an Orange Pi with the operating system being Armbian-based for compatibility with the OrangePi; this handles the DNS queries for the homelab.

Routing is handled at the gateway, and remote access into the homelab is handled through the zero-trust mesh network. Both of these are accessible through their own admin interface, with the option to tweak and change. All infrastructure services are designed with the idea of security, isolation, and resilience in mind, an attempt to reflect enterprise-grade principles. 


## Navigation
- [Rack Layout](https://github.com/joseankgarcia/homelab/blob/main/infrastructure/rack-layout.md)
    - [Diagram](https://github.com/joseankgarcia/homelab/blob/main/infrastructure/rack-layout.md/#diagram)
- [Hardware](https://github.com/joseankgarcia/homelab/blob/main/infrastructure/hardware.md)
    - [Primary Server](https://github.com/joseankgarcia/homelab/blob/main/infrastructure/hardware.md#primary-server)
    - [Secondary Server](https://github.com/joseankgarcia/homelab/blob/main/infrastructure/hardware.md#secondary-server)
- [Storage](https://github.com/joseankgarcia/homelab/blob/main/infrastructure/storage.md)
- [VLAN Design](https://github.com/joseankgarcia/homelab/blob/main/infrastructure/vlan-design.md)
