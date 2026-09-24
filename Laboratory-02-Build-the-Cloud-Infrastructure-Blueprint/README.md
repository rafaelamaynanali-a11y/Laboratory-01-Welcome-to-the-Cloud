# Laboratory 02 – Build the Cloud Infrastructure Blueprint

## Mission Overview

This laboratory activity focused on investigating the basic components of cloud infrastructure using the KillerCoda Playground. The Linux environment was examined to identify compute, storage, networking, and operating system resources. The findings were documented to help prepare a simple cloud infrastructure plan before deployment.

## Objectives

- Explain the major components of cloud infrastructure.
- Investigate hardware and software resources in a Linux environment.
- Differentiate compute, storage, networking, and operating system resources.
- Explain how infrastructure components work together.
- Compare services from AWS, Microsoft Azure, and Google Cloud.
- Create technical documentation using Markdown.

## Cloud Infrastructure Components

The investigated environment included a Linux operating system, a virtual CPU, memory, disk storage, mounted file systems, and a network interface. These resources represent the basic components needed to run applications in a cloud environment.

- **Compute:** The virtual CPU processes commands and runs applications.
- **Storage:** The virtual disk stores the operating system, files, and application data.
- **Networking:** The network interface and IP address allow communication between the server and other systems.
- **Operating System:** Ubuntu manages the hardware resources and provides the command-line environment.

## Tools Used

- KillerCoda Playground
- Ubuntu Linux terminal
- GitHub
- Markdown
- Screenshot tools
- Cloud architecture diagram

## Linux Commands Executed

The following commands were used during the investigation:

```bash
cat /etc/os-release
uname -r
lscpu
nproc
free -h
df -h
lsblk
hostname
ip a
