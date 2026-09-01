Continue Your Linux Investigation

## 1. Operating System

The Linux server is running **Ubuntu 24.04 LTS**.

The operating system information was collected using the `cat /etc/os-release` command.

![Operating System](screenshots/os-information.png)

---

## 2. CPU Information

The server uses an **Intel Xeon E312xx processor** with **1 CPU**.

The CPU information was collected using the `lscpu` command.

![CPU Information](screenshots/cpu-information.png)

---

## 3. Memory

The server has approximately **1.9 GiB of RAM**.

The memory information was collected using the `free -h` command.

![Memory Information](screenshots/memory-information.png)

---

## 4. Disk Space

The server has a **19 GB** root filesystem (`/dev/vda1`), with approximately **549 MB used** and **18 GB available**.

The disk information was collected using the `df -h` command.

![Disk Space](screenshots/disk-space.png)

---

## 5. Cloud Migration

If this Linux server were migrated to the cloud, the following services could be used to host the Linux server:

| Cloud Platform | Service | Purpose |
|---|---|---|
| AWS | Amazon EC2 | Host the Linux server as a virtual machine. |
| Microsoft Azure | Azure Virtual Machines | Host the Linux server as a virtual machine. |
| Google Cloud Platform | Compute Engine | Host the Linux server as a virtual machine. |

These services provide virtual computing resources that can run Linux-based workloads in the cloud. The Linux server can be migrated to a suitable virtual machine configuration based on its CPU, memory, storage, and workload requirements.
