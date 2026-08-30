# Cloud Infrastructure Components

## Compute Resources

**Purpose:**  
Compute resources provide the processing power needed to run applications, execute commands, and perform computing tasks.

**Importance in Cloud Computing:**  
Compute resources are important because cloud systems need processing power to run applications, services, and workloads.

**KillerCoda Linux Environment:**  
In my KillerCoda environment, the Intel Xeon E312xx processor represents the compute resource. The `lscpu` command showed that the environment has one CPU core.

## Storage Resources

**Purpose:**  
Storage resources provide space for storing the operating system, files, applications, and other data.

**Importance in Cloud Computing:**  
Storage is important because cloud systems need reliable space to store and access data.

**KillerCoda Linux Environment:**  
I used the `df -h` command to examine the storage resources in KillerCoda. The main `/dev/vda1` file system has a capacity of 19 GB.

## Networking Resources

**Purpose:**  
Networking resources allow computers, servers, and other cloud resources to communicate and exchange data.

**Importance in Cloud Computing:**  
Networking is important because it provides connectivity between users, servers, applications, and other cloud resources.

**KillerCoda Linux Environment:**  
I used the `hostname` and `hostname -I` commands to examine the hostname and IP addresses of the KillerCoda server.

## Operating System

**Purpose:**  
The operating system manages the hardware and software resources of the computer and provides an environment where applications and commands can run.

**Importance in Cloud Computing:**  
An operating system is important because cloud servers need it to manage resources and run applications and services.

**KillerCoda Linux Environment:**  
My KillerCoda server uses Ubuntu 24.04.4 LTS (Noble Numbat) with Linux kernel 6.8.0-138-generic.
