# Infrastructure Report

## 1. Operating System

The cloud server is running **Ubuntu Linux**. The Linux kernel version installed on the server is:

```text
6.8.0-136-generic
```

The operating system provides the environment required to run applications, manage system resources, and interact with the underlying cloud infrastructure.

## 2. CPU

The server uses an:

**Intel Xeon E312xx (Sandy Bridge, IBRS update)**

The system has **1 CPU core** available to the virtual machine.

The CPU is responsible for executing instructions and processing workloads running on the cloud server.

## 3. Memory

The server has approximately **1.9 GiB of total RAM**.

At the time of investigation:

- Used: 438 MiB
- Free: 843 MiB
- Available: 1.4 GiB
- Swap: 1.0 GiB

RAM is used by the operating system and applications for temporary data and active processes.

## 4. Disk Capacity

The server has a **20 GB virtual disk**, identified as `vda`.

The main partitions are:

- `vda1` – 19 GB, mounted at `/`
- `vda15` – 106 MB, mounted at `/boot/efi`
- `vda16` – 913 MB, mounted at `/boot`

The root filesystem has approximately 13 GB of available space at the time of investigation.

## 5. Mounted File Systems

The following filesystems were observed:

| Filesystem   | Size | Used | Available | Mount Point |
| ------------ | ---: | ---: | --------: | ----------- |
| tmpfs        | 191M | 996K |      190M | `/run`      |
| `/dev/vda1`  |  19G | 5.4G |       13G | `/`         |
| tmpfs        | 952M |  84K |      952M | `/dev/shm`  |
| tmpfs        | 5.0M |    0 |      5.0M | `/run/lock` |
| `/dev/vda16` | 881M | 117M |      703M | `/boot`     |
| `/dev/vda15` | 105M | 6.2M |       99M | `/boot/efi` |

These filesystems provide storage for the operating system, boot files, temporary system data, and other system resources.

## 6. Hostname

The hostname of the server is:

```text
ubuntu
```

A hostname provides a name by which the Linux system can be identified within its network environment.

## 7. IP Address

The server reports the following IP addresses:

```text
172.30.1.2
172.17.0.1
```

The `172.30.1.2` address is associated with the cloud environment, while `172.17.0.1` is commonly associated with a Docker/container networking interface.

## 8. Investigation Commands

The following Linux commands were used during the investigation:

```bash
uname -r
lscpu | grep "Model name"
nproc
free -h
lsblk
df -h
hostname
hostname -I
```

## 9. Summary

The KillerCoda environment provides a virtualized Linux cloud server with one CPU core, approximately 1.9 GiB of RAM, and a 20 GB virtual disk. The server uses Ubuntu Linux and has a hostname of `ubuntu`. These resources represent the basic compute, memory, storage, and networking infrastructure that would be assessed before deploying applications to a cloud environment.
