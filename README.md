# NFS Configuration Automation

Automate the setup and management of Network File System (NFS) shares between machines in a network using a simple shell script. This project streamlines file sharing by automating directory creation, mounting, file transfers, error handling, and cleanup — making NFS accessible for both beginners and professionals.

---

## Table of Contents

- [Introduction](#introduction)  
- [Features](#features)  
- [Prerequisites](#prerequisites)  
- [Setup and Configuration](#setup-and-configuration)  
- [Usage](#usage)  
- [Shell Script](#shell-script)  
- [Output and Verification](#output-and-verification)  
- [Conclusion](#conclusion)  
- [Contributing](#contributing)  
- [License](#license)

---

## Introduction

Network File System (NFS) allows remote directories to be accessed as if they were local, enabling seamless file sharing across systems. This project automates NFS configuration using a shell script to simplify tasks like creating mount points, mounting shares, copying files, error handling, and cleanup. It is designed to be user-friendly and reliable, even for users with minimal technical experience.

---

## Features

- Automated creation of mount directories if they don’t exist  
- Automated mounting of NFS shares from server to client  
- Automated file copying to the NFS-mounted directory  
- Robust error detection and handling with detailed logging  
- Automatic unmounting of NFS shares after operations  
- Logs all actions for accountability and troubleshooting  
- Scalable and adaptable to various network setups  
- Beginner-friendly shell script, easy to customize and extend

---

## Prerequisites

- Two machines (physical or virtual) connected on the same network  
- NFS packages installed on both server and client machines  
- Root or sudo privileges to run configuration commands  
- Network configured in bridged mode (for virtual machines)

---

## Setup and Configuration

### Server-side Configuration

1. Install NFS server packages:
   ```bash
   sudo apt install nfs-kernel-server
