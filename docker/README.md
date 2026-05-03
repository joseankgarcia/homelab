# Stack Overview

This stack overview documents the Docker images, containers, Compose files, and deployment structure used throughout the homelab environment.

- **Proxy** is responsible for ingress, reverse proxying, SSL, and controlling access to other services across the network. <br>
- **Core** is responsible for the foundational and central services that other containers rely on. <br>
- **Services** contains general-purpose containers/applications that do not fit within a specific category <br>
- **Monitoring** is responsible for collecting, visualizing, and presenting the system metrics, logs, and the external databases in a digestible format. <br>
- **Backup & Discovery** is responsible for backing up workflows, restoring processes, and service or asset discovery within the environment. <br>
- **RSS** is responsible for  RSS feed aggregation and syndication from various sources. <br>
- **Media** is responsible for media storage, organization, and viewing across the LAN.

## Navigation
- [Automation](https://github.com/joseankgarcia/homelab/tree/main/docker/automation.md)
- [Proxy](https://github.com/joseankgarcia/homelab/blob/main/docker/proxy.md)
- [Core](https://github.com/joseankgarcia/homelab/blob/main/docker/core.md)
- [Services](https://github.com/joseankgarcia/homelab/blob/main/docker/services.md)
- [Monitoring](https://github.com/joseankgarcia/homelab/blob/main/docker/monitoring.md)
- [Backup & Discovery](https://github.com/joseankgarcia/homelab/blob/main/docker/backup&monitoring.md)
- [RSS](https://github.com/joseankgarcia/homelab/blob/main/docker/rss.md)
- [Media](https://github.com/joseankgarcia/homelab/blob/main/docker/media.md)
