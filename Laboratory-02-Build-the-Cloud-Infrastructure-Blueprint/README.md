# Laboratory 02 – Build the Cloud Infrastructure Blueprint

## Mission Overview

This laboratory activity focused on investigating and documenting a cloud-based Linux server environment before deploying any services. Using the KillerCoda terminal, the Linux infrastructure was inspected to identify its operating system, kernel version, CPU, memory, disk capacity, mounted filesystems, hostname, and IP addresses. The collected information was then used to create a basic cloud infrastructure blueprint and compare equivalent infrastructure services offered by AWS, Microsoft Azure, and Google Cloud Platform.

## Objectives

- Investigate the configuration of a Linux server running in a cloud environment.
- Identify the compute, storage, networking, and operating system components of the server.
- Document the infrastructure findings using Markdown.
- Research equivalent infrastructure services from AWS, Microsoft Azure, and Google Cloud Platform.
- Design a simple cloud infrastructure diagram.
- Practice using Linux commands to inspect system resources.
- Organize and document the laboratory work in a GitHub repository.

## Cloud Infrastructure Components

The following infrastructure components were identified during the investigation:

### Compute Resources

The KillerCoda environment provides an **Intel Xeon E312xx (Sandy Bridge, IBRS update)** processor with **1 CPU core** and approximately **1.9 GiB of RAM**. These resources provide the processing and memory capacity required to execute applications and workloads.

### Storage Resources

The server has a **20 GB virtual disk** identified as `vda`. The main root partition is approximately 19 GB and is mounted at `/`, while additional partitions are used for `/boot` and `/boot/efi`.

### Networking Resources

The server has the IP addresses **172.30.1.2** and **172.17.0.1**. These addresses demonstrate the server's participation in virtualized network environments.

### Operating System

The server runs **Ubuntu Linux** with kernel version **6.8.0-136-generic**. The operating system manages the server's hardware and software resources and provides the environment for running applications and services.

## Tools Used

- **KillerCoda** – Used to access and investigate the Linux cloud environment.
- **Linux Terminal** – Used to execute system and networking commands.
- **Git and GitHub** – Used to organize, version, and publish the laboratory files.
- **Markdown** – Used to create the technical documentation.
- **Draw.io / Diagramming Tool** – Used to design the cloud infrastructure diagram.
- **AWS Official Documentation** – Used to research AWS infrastructure services.
- **Microsoft Azure Official Documentation** – Used to research Azure infrastructure services.
- **Google Cloud Official Documentation** – Used to research Google Cloud infrastructure services.

## Linux Commands Executed

The following commands were used to investigate the KillerCoda Linux server:

| Command                      | Purpose                                                            |
| ---------------------------- | ------------------------------------------------------------------ |
| `uname -r`                   | Displays the Linux kernel version.                                 |
| `lscpu \| grep "Model name"` | Displays the CPU model.                                            |
| `nproc`                      | Displays the number of available CPU processing units.             |
| `free -h`                    | Displays RAM and swap memory information in human-readable format. |
| `lsblk`                      | Displays block devices, disk partitions, and mount points.         |
| `df -h`                      | Displays filesystem capacity, usage, and available storage.        |
| `hostname`                   | Displays the hostname of the server.                               |
| `hostname -I`                | Displays the IP addresses assigned to the system.                  |
| `ip addr`                    | Displays network interfaces and their IP addresses.                |
| `cat /etc/os-release`        | Displays information about the installed Linux distribution.       |

## Skills Learned

Through this laboratory activity, I learned how to inspect a cloud-based Linux server using command-line tools. I gained practical knowledge about identifying CPU, memory, disk, filesystem, hostname, and networking information.

I also learned how fundamental infrastructure components such as compute, storage, networking, and operating systems work together in a cloud environment. Researching AWS, Azure, and Google Cloud helped me understand that different cloud providers offer similar infrastructure capabilities under different service names.

The activity also improved my technical documentation, Markdown, Git, GitHub, cloud infrastructure research, and basic cloud architecture design skills.

## Challenges Encountered

One challenge was understanding the information returned by different Linux commands and determining which values represented the actual cloud server resources. For example, the `lsblk` and `df -h` commands displayed multiple partitions and filesystems, which required careful interpretation.

Another challenge was understanding the equivalent services offered by different cloud providers because AWS, Azure, and Google Cloud use different names for similar infrastructure capabilities.

Creating the cloud infrastructure diagram also required organizing the components clearly while ensuring that all required elements—user, internet connection, network, compute, and storage—were included.

Despite these challenges, the investigation provided practical experience with Linux system administration, cloud infrastructure, technical documentation, and cloud architecture concepts.
