# Infrastructure Report

## System Information

**Operating System:** Ubuntu 24.04.4 LTS

**Kernel:** 6.8.0-136-generic

**Architecture:** x86_64

**CPU:** Intel Xeon E312xx (Sandy Bridge, IBRS update)

**CPU(s):** 1

**RAM:** 1.9 GiB

**Hostname:** ubuntu

**Main Network Interface:** enp1s0

**Server IP Address:** 172.30.1.2

## Storage Information

**Main Filesystem:** /dev/vda1

**Mount Point:** /

**Total Size:** 19G

**Used:** 5.4G

**Available:** 13G

**Usage:** 30%

## Network Information

The main network interface detected in the KillerCoda environment is `enp1s0`. Its assigned IPv4 address is `172.30.1.2/24`.

The `172.17.0.1` address belongs to the Docker virtual interface (`docker0`) and is not used as the main server IP for this laboratory documentation.

## Environment

The infrastructure information was collected from the Ubuntu virtual machine provided by the KillerCoda laboratory environment using Linux system commands.

## Commands Used

- `cat /etc/os-release`
- `uname -r`
- `lscpu`
- `free -h`
- `df -h`
- `hostname`
- `hostname -I`
- `ip addr`
