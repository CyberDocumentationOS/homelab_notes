# Week 6 — Day 1
# Hypervisors & Virtualization

---

# Warm-Up (Week 1 Review)

## Multiple Choice

### 1. Which command displays your current working directory?

A) ls

B) cd

C) pwd

D) mkdir

Answer: c

---

### 2. Which command lists files and directories?

A) touch

B) ls

C) pwd

D) sudo

Answer: b

---

### 3. Which command changes your current directory?

A) cd

B) mkdir

C) chmod

D) whoami

Answer: a

---

### 4. Which command creates a new directory?

A) touch

B) ls

C) mkdir

D) cp

Answer: c

---

### 5. Which command creates an empty file?

A) rm

B) mkdir

C) touch

D) cat

Answer: c

---

### 6. Which command changes file permissions?

A) chmod

B) chown

C) sudo

D) pwd

Answer: a

---

### 7. Which command shows the groups a user belongs to?

A) groups

B) mkdir

C) ls

D) cd

Answer: a

---

### 8. What does sudo allow a user to do?

A) Delete Linux

B) Run commands with elevated privileges

C) Create networks

D) Change IP addresses

Answer: b

---

### 9. Which permission string represents chmod 755?

A) rw-r--r--

B) rwxr-xr-x

C) rwx------

D) rwxrwxrwx

Answer: b

---

### 10. Which directory typically contains user home folders?

A) /etc

B) /var

C) /home

D) /bin

Answer: c

---

# Task 1 — What is Virtualization?

# Virtualization Fundamentals

---

## Multiple Choice

### What is virtualization?

A) Installing antivirus software

B) Creating virtual versions of computers and resources

C) Encrypting files

D) Managing user accounts

Answer: b

---

### What is a virtual machine (VM)?

A) A physical computer

B) A virtualized computer running inside another computer

C) A network cable

D) A Linux command

Answer: b

---

### What software commonly creates virtual machines?

A) Notepad

B) VirtualBox

C) Paint

D) Event Viewer

Answer: b

---

## Short Answer

### What is virtualization?
Virtualization is the process of creating virtual versions of physical computing resources. 
Note: Virtualization is the process of creating software-based versions of computing resources such as operating systems, servers, storage, or networks. (Graded)
---

### What is a virtual machine?
A virtual machine is a software-based emulation of a physical computer that operates as an isolated computing enviroment with its own virtual hardware. 
---

### Why is virtualization useful?
Virtualization is useful because it maximizes hardware efficiency, allowing multiple isolated virtual computing enviroments to run on a single physcial computing enviroment, saving money and time on physical hardware and space. 
---

## Fill In The Blanks

A virtual machine runs on top of a: Hypervisor.
---

The operating system installed directly on the physical computer is called the: host OS.
---

The operating system running inside a virtual machine is called the: guest OS.
---

A virtual machine behaves like a: virtual computer with it's own virtual hardware.
---

## Host OS vs Guest OS

### Host OS
The host OS is the operating system that is directly on the physcial computer. 

---

### Guest OS
The guest OS is the operating system that is running inside a virtual machine, through something like VirtualBox or VMWare. 

---

## Short Answer

### What is the difference between a host OS and a guest OS?
The host OS is the operating system that is directly on the hardware itself, while a guest OS runs inside a virtual machine like VirtualBox. 
---

### Can a host machine run multiple guest operating systems at once?

A) Yes

B) No

Answer: a

---

### Why might cybersecurity professionals use virtual machines?
A cybersecurity professional might use a virtual machine to test certain programs/methods without harming the physical computer, or to run a program/process in an isolated enviroment. 
---

# In Your Own Words

### Explain virtualization to a beginner.
Virtualization is the process of creating virutal versions of computing resources. 
Note: Virtualization lets one computer pretend to be several separate computers. (Graded)
---

### Explain what a virtual machine is.
A virtual machine is an isolated softwar-based emulation of an operating system with it's own virtual components. 
---

### Explain the difference between a host OS and a guest OS.
The host OS is the operating system that is running on the physical hardware, while the guest OS is an operating system running on a virtual machine like VirtualBox. 
---

# Task 2 — Hypervisors

# Hypervisors

---

## Multiple Choice

### What is a hypervisor?

A) A web browser

B) Software that manages virtual machines

C) A Linux command

D) A registry hive

Answer: b

---

### What is the primary purpose of a hypervisor?

A) Create and manage virtual machines

B) Browse the internet

C) Manage user passwords

D) Encrypt files

Answer: a

---

## Hypervisor Types

### Type 1 Hypervisor

Runs: directly on the physical hardware without requiring an underlying host OS. 
---

### Type 2 Hypervisor

Runs: on an existing host operating system. 
---

## Multiple Choice

### Which hypervisor type runs directly on hardware?

A) Type 1

B) Type 2

Answer: a

---

### Which hypervisor type runs on top of an operating system?

A) Type 1

B) Type 2

Answer: b

---

### VirtualBox is which type of hypervisor?

A) Type 1

B) Type 2

Answer:  b

---

## Short Answer

### What is a Type 1 hypervisor?
A type 1 hypervisor is a virtualization software that runs directly on the hardware itself, without needing an underlying host OS. 
---

### What is a Type 2 hypervisor?
A type 2 hypervisor is a virtualization software that runs on top of a host OS. 
---

### Why is VirtualBox considered a Type 2 hypervisor?
VirtualBox is considered a type 2 hypervisor because the application itself runs on a host OS, like Windows. 
---

### Why are hypervisors useful?
Hypervisors are useful because they enable server virtualization, allowing for multiple virtual machines to run on a single physical server. 
Note: Hypervisors allow multiple isolated virtual machines to share the same physical hardware efficiently while keeping them separated from one another. (Graded)
---

## Examples

### Type 1 Hypervisors

List examples:

1. VMware ESXi

2. Hyper-V

3. KVM (Kernel-based Virtual Machine)

---

### Type 2 Hypervisors

List examples:

1. VirtualBox

2. VMware Workstation

3. Parallels Desktop

---

## Fill In The Blanks

VirtualBox is a:

type 2 hypervisor.

---

VMware ESXi is a:

type 1 hypervisor.

---

Hypervisors allow multiple:

virtual machines to run on one physical computer.

---

# In Your Own Words

### Explain what a hypervisor does.
A hypervisor is virtualization software that allows a virtual machine to run on a physical computer.
Note: A hypervisor creates, manages, and allocates hardware resources to virtual machines running on a physical computer. (Graded) 
---

### Explain the difference between Type 1 and Type 2 hypervisors.
A type 1 hypervisor runs on the physical hardware directly, while a type 2 hypervisor runs on top of a host OS. 
---

### Why are hypervisors important in cybersecurity?
Hypervisors are important in cybersecurity because they allow the isolated testing of methods and safe interrogation of potenial malicious software. 
---

# Task 3 — VM Inventory

# VM Inventory

---

## Host Machine Information

### Host Operating System
Windows 11 Home Edition
---

### CPU
11th Gen Intel(R) Core(TM) i5-11400H @ 2.70GHz
---

### RAM
16.0 GB installed RAM
---

### Storage
477 GB
---

### Hypervisor Software
VirtualBox
Type 2 Hypervisor
---

# Existing Virtual Machines

List every VM you currently have available.

| VM Name | OS | Purpose |
| Linux Practice | Ubuntu | To learn and practice Linux. |
| Linux Mint | MintOS | To fiddle around with MintOS and try new things. |
| Kali Linux | Kali | To learn and practice Kali/Cybersecurity techniques. |

---

# Planned Virtual Machines

List the VMs you plan to create.

| VM Name | OS | Purpose |
| Windows 10 | Windows 10 | To learn and practice homelabbing. |
| Windows Server | Windows Server 2022 | To fiddle around and explore server (just for fun). |

---

## Short Answer

### Which VM do you think will be most useful for cybersecurity?
Kali Linux is a cybersecurity focused version of linux, so I think that is going to be the most useful in the end. 
---

### Which VM do you think will be the most difficult to learn?
Kali Linux because it is very cybersecurity focused, and things like password cracking seem like that are going to be difficult to do at first. 
---

### Why is it useful to have multiple operating systems available?
Having multiple operating systems available allows you to dedicate specific tasks to isolated machines, ensuring it doesn't interfere with anything else important. 
---

# Reflection

### What is one thing you learned about virtualization today?
I learned that virtualization is the process of creating virtual versions of physical computer hardware.
---

### What is one thing you learned about hypervisors?
I learned that there are 2 types of hypervisors, and that VirtualBox is a type 2 hypervisor. 
---

### What is one thing you want to learn more about?
This is way, way, WAY in the future, but I would be interesting in learned about viruses that are able to escape VMs, which seems like some very advanced and scary stuff. 
---

