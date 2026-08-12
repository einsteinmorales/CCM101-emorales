## Linux Server Investigation

For this checkpoint, a Linux server was launched using a **KillerCoda Playground**. Linux commands were used to identify the operating system, CPU information, memory, and disk space.

## 1. Operating System

The following command was used:

```bash
cat /etc/os-release
```

### Result

* **Operating System:** Ubuntu 24.04.4 LTS
* **Version:** 24.04.4 LTS
* **Codename:** Noble Numbat
* **Architecture:** x86_64

### Screenshot

![Operating System](screenshots/linux/os-release.png)

---

## 2. CPU Information

The following command was used:

```bash
lscpu
```

### Result

* **CPU:** Intel Xeon E312xx (Sandy Bridge)
* **CPU(s):** 1
* **Core(s) per socket:** 1
* **Architecture:** x86_64
* **Virtualization:** KVM

### Screenshot

![CPU Information](screenshots/linux/lscpu.png)

---

## 3. Memory

The following command was used:

```bash
free -h
```

### Result

* **Total Memory:** 1.9 GiB
* **Used Memory:** 412 MiB
* **Free Memory:** 874 MiB
* **Available Memory:** 1.5 GiB
* **Swap:** 1.0 GiB

### Screenshot

![Memory Information](screenshots/linux/memory.png)

---

## 4. Disk Space

The following command was used:

```bash
df -h
```

### Result

The main filesystem `/dev/vda1` has:

* **Total Size:** 19 GB
* **Used:** 5.4 GB
* **Available:** 13 GB
* **Usage:** 30%

### Screenshot

![Disk Space](screenshots/linux/disk-space.png)

---

# Cloud Migration

If this Linux server were migrated to the cloud, it could be hosted using virtual machine services from AWS, Microsoft Azure, or Google Cloud Platform.

| Cloud Provider      | Cloud Service          | Purpose                      |
| ------------------- | ---------------------- | ---------------------------- |
| **AWS**             | Amazon EC2             | Hosts Linux virtual machines |
| **Microsoft Azure** | Azure Virtual Machines | Hosts Linux servers          |
| **GCP**             | Compute Engine         | Hosts Linux virtual machines |

## AWS – Amazon EC2

**Amazon EC2** can host the Ubuntu Linux server as a virtual machine. CPU, memory, storage, and networking resources can be configured according to the server's requirements.

## Microsoft Azure – Azure Virtual Machines

**Azure Virtual Machines** can run Ubuntu Linux servers in Microsoft's cloud infrastructure. It allows users to select the required virtual machine size and storage.

## GCP – Compute Engine

**Google Compute Engine** can host the Ubuntu server as a virtual machine. It provides configurable CPU, memory, storage, and networking resources.

---

# Summary

| Category             | Information Collected |
| -------------------- | --------------------- |
| **Operating System** | Ubuntu 24.04.4 LTS    |
| **Architecture**     | x86_64                |
| **CPU**              | Intel Xeon E312xx     |
| **CPU Cores**        | 1                     |
| **Memory**           | 1.9 GiB               |
| **Available Memory** | 1.5 GiB               |
| **Disk**             | 19 GB                 |
| **Disk Used**        | 5.4 GB                |
| **Disk Available**   | 13 GB                 |

The Linux server can be migrated to **Amazon EC2, Azure Virtual Machines, or Google Compute Engine**. All three services support Ubuntu Linux and allow the server resources to be adjusted based on the application's needs.

## Screenshot Folder

The screenshots are organized as follows:

```text
screenshots/
└── linux/
    ├── os-release.png
    ├── lscpu.png
    ├── memory.png
    └── disk-space.png
```

