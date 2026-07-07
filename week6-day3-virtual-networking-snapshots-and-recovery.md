# Week 6 — Day 3 (Combined Day 3 & 4)
# Virtual Networking, Snapshots & Recovery

---

# Warm-Up (Week 3 Review)

## Multiple Choice

### 1. What is the primary purpose of an IP address?

A) Identify a file

B) Identify a device on a network

C) Identify a user

D) Encrypt data

Answer: b

---

### 2. Which device primarily forwards traffic between different networks?

A) Switch

B) Router

C) Firewall

D) Access Point

Answer: b

---

### 3. Which device forwards traffic using MAC addresses?

A) Router

B) Switch

C) DNS Server

D) DHCP Server

Answer: b

---

### 4. What does DNS do?

A) Assign IP addresses

B) Encrypt web traffic

C) Translate domain names into IP addresses

D) Route packets

Answer: c

---

### 5. What does DHCP do?

A) Assign IP addresses automatically

B) Resolve domain names

C) Encrypt traffic

D) Scan ports

Answer: a

---

### 6. Which address is commonly used by a home router?

A) 8.8.8.8

B) 127.0.0.1

C) 192.168.1.1

D) 255.255.255.255

Answer: c

---

### 7. Which subnet mask is commonly used for home networks?

A) 255.255.255.0

B) 255.0.0.0

C) 255.255.0.0

D) 255.0.255.0

Answer: a

---

### 8. Which command shows IP addresses in Ubuntu?

A) pwd

B) ip addr

C) ls

D) chmod

Answer: b

---

### 9. Which device usually assigns IP addresses on a home network?

A) Router

B) Switch

C) Computer

D) DNS Server

Answer: a

---

### 10. Which networking component translates website names into IP addresses?

A) DHCP

B) DNS

C) Router

D) Switch

Answer: b

---

# Task 1 — Virtual Networking Modes

# Virtual Networking

---

## Multiple Choice

### What is NAT networking?

A) A networking mode that hides the VM behind the host's network connection

B) A physical network cable

C) A Linux command

D) A Windows service

Answer: a

---

### What is Bridged networking?

A) A networking mode that gives the VM its own presence on the physical network

B) A backup system

C) A firewall

D) A storage device

Answer: a

---

### What is Host-Only networking?

A) A networking mode where the VM communicates only with the host (and other Host-Only VMs)

B) Internet-only networking

C) Wireless networking

D) Bluetooth networking

Answer: a

---

## Short Answer

### What is NAT?
NAT (Network Address Translation) is a networking technology that maps private IP addresses to public IP addresses, allowing for multiple devices on a network to share a single IP address.
---

### What is Bridged networking?
Bridged networking is a configuration where a VM or container appears as a unique independent device on the same network as the host OS. 
---

### What is Host-Only networking?
Host-only networking is a virtual network configuration that creates a private, isolated environment allowing the VMs and host computer to communicate while blocking access to the external internet. 
---

### Why is virtualization networking important?
Virtualization networking is important because it seperates network functions from physical hardware, allowing you to manage, scale, and secure your infrastructure through software. 
Note: Virtualization networking allows virtual machines to communicate with each other, the host, and external networks while keeping them isolated and secure. (Graded)
---

## Fill In The Blanks

NAT stands for:
Network Address Translation.
---

Bridged networking allows a VM to appear as a:
Unique Independent device on the physical network.
---

Host-Only networking allows communication between:
Virtual Machines and the host system.
---

NAT networking allows VMs to access the:
internet/external networks without exposing them directly.
---

## Networking Modes

### NAT
Purpose:
The purpose of NAT is to conserve public IPv4 addresses by allowing multiple devices on a network to share a singular address. 
Note: Allow the VM to safely access the Internet while remaining hidden behind the host. (Graded)
---

### Bridged
Purpose:
The purpose of bridged networks is to have the VM be identifiable as it's own device on the same network as the host OS to reduce traffic congestion and improve overall performance. 
---

### Host-Only
Purpose:
The purpose of Host-Only networking is to have an isolated environment allowing the VMs and host OS to communicate while blocking access to the external internet, which is used for things like secure testing, development, and malware analysis.
---

## Short Answer

### Which networking mode is generally safest for beginners?
NAT is the safest mode for beginners because it shares the host's internet connection while remaining hidden behind, preventing external devices on the local network from accessing or scanning the VM. 
---

### Which networking mode would you use if another computer needed to access your VM?
Bridged networking is the best mode to use in this scenario, as using this mode, the VM is seen as a unique device and gets an IP address of its own, allowing for other devices to access the VM if needed. 
---

### Why do cybersecurity professionals use different networking modes?
Cybersecurity professionals use different networking modes to help limit attack surfaces, contain breaches, and analyze potential malware. 
---

# In Your Own Words

### Explain NAT networking to a beginner.
NAT networking is a networking mode that maps private IP addresses to public ones, allowing multiple devices to share the same IP address on the same network.
Note: Through the host computer. (Graded)
---

### Explain Bridged networking to a beginner.
Bridged networking is a networking mode that allows a VM/container to appear as a unique independent device on the same networking as the host OS.
---

### Explain Host-Only networking to a beginner.
Host-Only networking is a networking mode that allows VMs and the host OS to communicate in an isolated environment while blocking external internet access.
---

# Task 2 — Comparing Networking Modes

# Networking Lab

---

## Lab Instructions

Inside Ubuntu:

```bash
ip addr
```

Record your IP address while using:

- NAT
- Host-Only

---

## NAT Mode

### IP Address

Answer: 10.0.2.15

---

### Could the VM access the Internet?

A) Yes

B) No

Answer: a

---

## Host-Only Mode

### IP Address

Answer: 192.168.56.101

---

### Could the VM access the Internet?

A) Yes

B) No

Answer: b

---

## Observation Questions

### Did the IP address change?
Yes, the IP address did change when switching from NAT to host-only.
---

### Which IP address range did NAT use?
NAT used 10.0.2.15 as it's IP address, so it used the 10.0.2.x range.
---

### Which IP address range did Host-Only use?
Host-Only used 192.168.56.101 as it's IP address, so it used the 192.168.56.x range. 
---

### Which networking mode seems safest for a cybersecurity lab?
I would say the safest networking mode is Host-Only because is creates an enviroment isolated from the network, allowing you to test malware and other things without risk of harming the actual network. 
---

## Fill In The Blanks

Host-Only networking isolates the VM from the:
internet. 
---

Bridged networking connects the VM directly to the:
local network.
---

NAT networking shares the host's:
IP address.
---

## In Your Own Words

### Explain why Host-Only networking is useful in cybersecurity.
Host-Only networking is useful in cybersecurity because it creates an environment isolated from the internet, allowing you to interact with potential malware without harming the actual network. 
---

### Explain why NAT is commonly used.
NAT is commonly used to conserve public IP addresses and enhance security by hiding the internal VM topologies from external networks. 
Note: NAT is commonly used because it allows virtual machines to access the Internet without exposing them directly to the local network. (Graded)
---

# Task 3 — Snapshots

# Virtual Machine Snapshots

---

## Multiple Choice

### What is a VM snapshot?

A) A screenshot

B) A saved state of a virtual machine

C) A backup of Windows

D) A networking protocol

Answer: b

---

### Why are snapshots useful?

A) They permanently increase storage

B) They allow a VM to be restored to an earlier state

C) They improve CPU speed

D) They replace antivirus software

Answer: b

---

## Short Answer

### What is a snapshot?
A snapshot is a saved state of a virtual machine at a specific moment that acts as a temporary restore point. 
---

### What does a snapshot capture?
A snapshot captures a point-in-time copy of the state a VM was in, recording the exact configurations at that moment. 
---

### Why are snapshots useful?
Snapshots are useful because they enable rapid, point in time recovery if something on the VM goes awry.
---

### When would a cybersecurity professional create a snapshot?
A cybersecurity professional would create a snapshot before experimenting with something like malware analysis or potential system breaking techniques in order to quickly reinstate the system afterwards. 
---

## Fill In The Blanks

A snapshot records the VM's:
point-in-time configurations and set up.
---

Snapshots allow you to return to a previous:
VM state.
---

Snapshots are useful before installing:
system updates
or
system altering applications.
---

## Multiple Choice

### What happens if you restore a snapshot?

A) The VM returns to the saved state

B) Windows reinstalls

C) RAM increases

D) Networking changes permanently

Answer: a

---

### Should snapshots replace backups?

A) Yes

B) No

Answer: b

---

## In Your Own Words

### Explain snapshots to someone new to virtualization.
Snapshots are saved states of virtual machines that act as temporary restore points for the system. 
---

### Explain why snapshots are valuable during penetration testing.
Snapshots are valuable during penetration testing because it allows you to go back to a previous saved state if you mess something up while in the pentesting process, allowing you to practice without having to reinstall the VM every time. 
---
