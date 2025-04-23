# DevOps-Task0

This repository contains the setup and steps for completing the initial DevOps task. Follow the instructions below to set up the environment, install required tools, and document the process.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Repository Setup](#repository-setup)
3. [Environment Setup](#environment-setup)
4. [Required Tools Installation](#required-tools-installation)
5. [Screenshots](#screenshots)
6. [Pull Request](#pull-request)

---

## Introduction
This task involves creating a private GitHub repository, setting up a UNIX-like operating system, and installing essential tools such as Docker, Terraform, Git, and more. The goal is to familiarize yourself with the environment and document the process thoroughly.

---

## Repository Setup
1. **Create a Private Repository:**
   - Repository Name: `DevOps-Task0`
   - Set it as private.

2. **Add Mentors as Collaborators:**
   - Add the following users:
     - `Ariiia`
     - `khrystynapavlyk1`
     - `1100-git`
     - `b-kostenko`

3. **Create `.gitignore` File:**
   - Add rules to ignore unnecessary files such as:
     ```
     *.env
     node_modules/
     .DS_Store
     *.log
     ```

4. **Create `DO_0` Branch:**
   - Use the following commands:
     ```bash
     git checkout -b DO_0
     git push origin DO_0
     ```

5. **Add README and Screenshot Folder:**
   - Create `README.md` (this file).
   - Create a folder named `screenshots/` to store images.

6. **Commit and Push Changes:**
   ```bash
   git add .
   git commit -m "Initial setup for DevOps-Task0"
   git push origin DO_0
   ```

---

## Environment Setup
1. **Install Virtualization Tool:**
   - Recommended tools:
     - [VirtualBox](https://www.virtualbox.org/)
     - [VMware Workstation Player](https://www.vmware.com/products/workstation-player.html)
     - [Hyper-V](https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/about/)

2. **Install UNIX-Like OS:**
   - Recommended OS: **Ubuntu 24.04**.
   - Install it on your virtual machine.

3. **Configure the OS:**
   - Update the system:
     ```bash
     sudo apt update && sudo apt upgrade -y
     ```

---

## Required Tools Installation

1. **Docker:**
   ```bash
   sudo apt install docker.io
   ```

2. **Docker Compose:**
   ```bash
   sudo apt install docker-compose
   ```

3. **Terraform:**
   ```bash
   curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -
   sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
   sudo apt update && sudo apt install terraform
   ```

4. **Git and GitHub CLI:**
   ```bash
   sudo apt install git
   sudo apt install gh
   ```

5. **Nginx:**
   ```bash
   sudo apt install nginx
   ```

6. **AWS CLI:**
   ```bash
   curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
   unzip awscliv2.zip
   sudo ./aws/install
   ```

---

## Screenshots
Below are placeholders for screenshots. Replace them with actual links once uploaded.

### Repository Creation
![Repository Creation](screenshots/repository_creation.png)

### Adding Collaborators
![Adding Collaborators](screenshots/adding_collaborators.png)

### Virtual Machine Setup
![Virtual Machine Setup](screenshots/virtual_machine_setup.png)

### Tools Installation
![Tools Installation](screenshots/tools_installation.png)

---

## Pull Request
1. Push changes to the `DO_0` branch:
   ```bash
   git push origin DO_0
   ```

2. Create a Pull Request (PR) from `DO_0` to the `main` branch.
   - Assign mentors to review the PR.

---

## Notes
- Ensure all commands work as expected.
- Document any issues encountered and how they were resolved.
- Keep the `README.md` updated with accurate information.
