# Laboratory 02 – Build the Cloud Infrastructure Blueprint

## Mission Overview

This laboratory focused on investigating the basic components of cloud infrastructure using the KillerCoda Linux virtual machine environment. The activity involved examining system resources, identifying compute, storage, networking, and operating system components, comparing major cloud providers, and creating a simple cloud infrastructure diagram.

## Objectives

- Explain the major components of cloud infrastructure.
- Investigate hardware and software resources in a Linux environment.
- Identify compute, storage, networking, and operating system resources.
- Compare equivalent infrastructure services from AWS, Microsoft Azure, and Google Cloud Platform.
- Create a simple cloud infrastructure diagram.
- Document technical findings using Markdown.
- Organize and maintain the GitHub Cloud Computing Portfolio.

## Cloud Infrastructure Components

### Compute

The compute resource used in the laboratory is a virtual machine running in the KillerCoda environment. It provides 1 virtual CPU using an Intel Xeon E312xx processor and provides the processing capacity needed to run the Linux operating system and laboratory tasks.

### Storage

The main storage resource identified is `/dev/vda1`, which has a total capacity of approximately 19 GB. It provides space for the Ubuntu operating system, files, applications, and other data required by the virtual machine.

### Networking

The main network interface is `enp1s0`, with the server IP address `172.30.1.2/24`. The network provides connectivity for the virtual machine and allows communication between the system and other resources.

### Operating System

The virtual machine runs Ubuntu 24.04.4 LTS with the Linux kernel version `6.8.0-136-generic` on an x86_64 architecture. The operating system manages the system resources and provides the environment for executing the laboratory commands.

## Tools Used

- KillerCoda Playground
- Ubuntu Linux
- Linux terminal
- GitHub
- Web browser
- diagrams.net (Draw.io)
- Markdown

## Linux Commands Executed

The following Linux commands were used to investigate the virtual machine:

- `cat /etc/os-release` – identifies the operating system.
- `uname -r` – displays the Linux kernel version.
- `lscpu` – displays CPU information and the number of CPU cores.
- `free -h` – displays memory information.
- `df -h` – displays disk and filesystem usage.
- `hostname` – displays the hostname.
- `hostname -I` – displays the system IP addresses.
- `ip addr` – displays network interface and IP address information.

## Skills Learned

This activity improved my skills in checking Linux system resources, identifying cloud infrastructure components, comparing cloud services, creating a basic infrastructure diagram, writing Markdown documentation, and managing files and commits in GitHub.

## Challenges Encountered

One challenge I encountered was interpreting the results from different Linux commands because some outputs contained more technical details than I needed. I had to carefully check the results to find the correct CPU, memory, storage, network, and operating system information required for the report. I also needed to make sure that my files, screenshots, and architecture diagram were placed in the correct folders and had the required filenames.
