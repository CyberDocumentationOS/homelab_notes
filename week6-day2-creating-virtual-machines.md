# Week 6 Day 2 — Creating Virtual Machines

# Warm-Up (Week 2 Review)

## Multiple Choice

### 1. Which command changes file permissions?

A) chown

B) chmod

C) groups

D) sudo

Answer: b

---

### 2. Which command changes the owner of a file?

A) chmod

B) chown

C) pwd

D) touch

Answer: b

---

### 3. Which permission allows reading a file?

A) w

B) x

C) r

D) s

Answer: c

---

### 4. Which permission allows modifying a file?

A) r

B) w

C) x

D) d

Answer: b

---

### 5. Which permission allows a file to be executed?

A) r

B) w

C) x

D) e

Answer: c

---

### 6. Which command displays the groups a user belongs to?

A) id

B) groups

C) whoami

D) sudo

Answer: b

---

### 7. What does `sudo` allow a user to do?

A) Create virtual machines

B) Run commands with elevated privileges

C) Delete user accounts automatically

D) Change network settings permanently

Answer: b

---

### 8. Which numeric permission corresponds to `rwxr-xr-x`?

A) 644

B) 777

C) 755

D) 600

Answer: c

---

### 9. Which Linux command displays your current username?

A) id

B) groups

C) whoami

D) pwd

Answer: c

---

### 10. Why is the principle of least privilege important?

A) It speeds up Linux

B) It gives everyone administrator access

C) It limits damage if an account is compromised

D) It increases RAM

Answer: c

---

# Task 1 — Kali VM

# Kali Linux Virtual Machine

---

## Multiple Choice

### What is Kali Linux?

A) A Windows utility

B) A Linux distribution designed for cybersecurity

C) A web browser

D) A hypervisor

Answer: b

---

### What organization develops Kali Linux?

A) Microsoft

B) Canonical

C) Offensive Security

D) VMware

Answer: c

---

### Which package manager does Kali Linux use?

A) yum

B) apt

C) pacman

D) dnf

Answer: b

---

## VM Configuration

### VM Name
Kali Linux
---

### RAM Allocated
6102 mb
---

### CPU Cores
6 Processors
---

### Storage Size
20 Gb
---

### Network Adapter
Intel PRO/100 MT Desktop (NAT)
---

## Short Answer

### What is Kali Linux?
Kali Linux is a special, Debian-based Linux distribution that is designed for penetration testing, digital forensics, and ethical hacking. 
---

### Why is Kali Linux commonly used in cybersecurity?
Kali Linux is used commonly in cybersecurity due to its focus on Red Team cybersecurity like penetration testing and ethical hacking. 
---

### What is the advantage of using Kali inside a virtual machine?
The advantage gained by using a Kali VM is safe isolation and Sandboxed testing, allowing you to test certain exploits, methods, and programs within a safe enviroment, not letting the physical hardware be harmed in the process. 
---

### What organization maintains Kali Linux?
The organization that maintains Kali Linux is Offensive Security (OffSec), which is an international information security company. 
---

# Kali Linux Tools

## Fill In The Blanks

Kali Linux comes preinstalled with many:
cybersecurity tools designed for pentesting, digital forensics, security research, and reverse engineering. 
---

One popular network scanning tool included with Kali is:
Nmap. 
---

A popular packet analysis tool included with Kali is:
Wireshark.
---

A popular password auditing tool included with Kali is:
John the Ripper.
---

## Short Answer

### Name three tools included with Kali Linux.

1. Nmap

2. Crunch

3. Hydra

---

### Which tool are you most interested in learning?
The John the Ripper tool sounds very interesting, and I would be interested in checking that out. 
---

### Why do cybersecurity professionals prefer Kali over installing tools one-by-one?
Installing Kali Linux makes it easier for cybersecurity professionals because over 600 tools are built into the distro itself, making it much more convenient in the long run. 
---

# In Your Own Words

### Explain what Kali Linux is to a beginner.
Kali Linux is a Debian-based Linux distro that has over 600 in Red Team cybersecurity tools built in. 
Note: Kali Linux is a Linux operating system built specifically for cybersecurity professionals and penetration testers, with hundreds of security tools already installed. (Graded)
---

### Explain why running Kali in a VM is safer than installing it directly onto your computer.
Installing a Kali VM allows you to test tools, exploits, and methods in a safe isolated environment, allowing you to test things without the risk of damaging the hardware itself. 
---

# Task 2 — VM Settings

# Virtual Machine Resources

---

## Multiple Choice

### Which resource determines how many calculations a VM can perform at once?

A) RAM

B) CPU

C) Storage

D) Network Adapter

Answer: b

---

### Which resource stores programs and files permanently?

A) CPU

B) RAM

C) Storage

D) GPU

Answer:  c

---

### Which resource temporarily stores data while programs are running?

A) Storage

B) RAM

C) CPU

D) BIOS

Answer: b

---

## Resource Allocation

### RAM Assigned
6102 Mb
---

### CPU Cores Assigned
6 Processors
---

### Storage Allocated
20 Gb

---

### Video Memory
16 Mb
---

## Fill In The Blanks

Giving a VM too much RAM can:
make the host OS sluggish.
---

Giving a VM too little RAM can:
make the guest OS sluggish.
---

Giving a VM too many CPU cores can:
cause performance degradation.
---

Giving a VM too little storage can:
cause the guest OS to run slowly. 
---

## Short Answer

### What happens if too much RAM is assigned to a VM?
When too much RAM is assigned to a VM, it can cause host OS system thrashing and VM performance degradation. Basically, it slows down the host OS and can make it sluggish. 
Note: When it comes to degradation, usually the host OS suffers more. (Graded)
---

### What happens if too little RAM is assigned?
When too little RAM is assigned to a VM, it can cause the guest OS to operate sluggishly and slow, making it difficult to use. 
---

### Why shouldn't you assign every CPU core to a VM?
You shouldn't assign every CPU core to a VM because you risk starving the host OS of system resources needed for background tasks, which can lead to system instability. 
---

### Why is storage planning important?
Storage planning is important because it prevents overprovisioning and underprovisioning, avoiding potential problems. 
---

## Observation Questions

### Which VM setting do you think is most important?
I think the storage allocation settings are the most important due to the fact that it can cause problems if you don't do it right. 
Note: RAM, CPU, Storage is correct order. (Graded)
---

### Which setting was easiest to understand?
I would say RAM allocation was the easiest to understand, as I did have a problem with it before when setting up the Ubuntu VM (2 Mb wasn't enough, so I had to do 6), so I know how to handle it now. 
---

### Which setting was most confusing?
I would say the most confusing setting is the Video Memory, not because it is difficult, more so that I haven't used it for anything yet. 
---

### Did any recommended settings surprise you?
Not really, they all seem pretty standard for a VM.
---

# In Your Own Words

### Explain why CPU, RAM, and storage all matter when creating a virtual machine.
CPU, RAM, and storage all matter when creating a VM because doing the incorrect amount of each can cause system instability on the guest OS, host OS, or both depending on the problem. It is important to get the correct amount of each to ensure a stable, usable environment. 
---

### Explain resource allocation to someone who has never used virtualization before.
Resource allocation is the practice of equalling out how much of a resource is given for a virtual machine. Doing the practice ensures that the virtual machine is given the proper amount of resources to run efficiently and safely. 
Note: It is basically deciding how much of each hardware resource is assigned to the virtual machine. (Graded)
---
