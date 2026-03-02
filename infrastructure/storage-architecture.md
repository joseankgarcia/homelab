# Storage Architecture

### Storage Overview
The storage architecture separates system disks through the use of mounting points in a central location. This makes diagnosing storage mounts, accessibility, and even implementing least privilege through TrueNAS ACL, making it more efficient and streamlined. 

## Primary Server
### Proxmox (Host)
- ```Hard Disk (scsio)``` : ```1tb NVMe```
- ```Hard Disk (virtio1)``` : ```4tb HDD```
- ```Hard Disk (virtio2)``` : ```4tb HDD```

notes: <br> 
``` scsio is the boot drive for Proxmox  ```
<br>
``` virtio1 and virtio2 are the drives that are passed to TrueNAS  ```
</br>

### TrueNAS VM
Drives
- ```Hard Disk (scsio)``` : ```50gb NVMe```
- ```Hard Disk (virtio1)``` : ```4tb HDD```
- ```Hard Disk (virtio2)``` : ```4tb HDD```

Mount Path
- ```Mount Point```:```/mnt/data```

Data Protection
- ``` data vdev configured in mirror on truenas ```
- ``` scrub tasks enabled on truenas ```

notes: <br> 
``` virtio passed from Proxmox to TrueNAS ```
<br>
``` scsio portion allocated from the Proxmox boot drive ```
<br>
```data mount point configured in truenas smb shares```
</br>

### Docker VM
Drives
- ```Hard Disk (scsio)``` : ```200gb NVMe```

Mount Path
- ```Mount Point```:```/mnt/data```

notes: <br> 
``` scsio portion allocated from the Proxmox boot drive ```
<br>
```data mount point configured in /etc/fstab```
</br>

## Secondary Server
### OrangePi
Drives
- ```Hard Disk``` : ```16gb MicroSD```

notes: <br> 
``` MicroSD is the boot drive for the OrangePi  ```


