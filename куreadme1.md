# DevOps-Task0


---

## Table of Contents
1. [Introduction](#introduction)
2. [Repository Setup](#repository-setup)
3. [Environment Setup](#environment-setup)
4. [Required Tools Installation](#required-tools-installation)
5. [Screenshots](#screenshots)

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
   - Recommended tool:
     - [VirtualBox](https://www.virtualbox.org/)
    
2. **Install UNIX-Like OS:**
   - Recommended OS: **Ubuntu 24.04**.
   - Install it on virtual machine.

3. **Configure the OS:**
   - Update the system:
     ```bash
     sudo apt update && sudo apt upgrade -y
     ```

---

## Required Tools Installation

1. **Docker and Docker Compose:**
   ```bash
   sudo apt install docker.io -y
    DOCKER_CONFIG=${DOCKER_CONFIG:-$HOME/.docker}
    mkdir -p $DOCKER_CONFIG/cli-plugins
     curl -SL https://github.com/docker/compose/releases/download/v2.35.0/docker-compose-linux-x86_64 -o $DOCKER_CONFIG/cli-     plugins/docker-compose
   chmod +x $DOCKER_CONFIG/cli-plugins/docker-compose 
   docker --version
   docker-compose --version
   ```

2. **Terraform:**
   ```bash
   sudo apt-get update && sudo apt-get install -y gnupg software-properties-common
    wget -O- https://apt.releases.hashicorp.com/gpg | \
    gpg --dearmor | \
    sudo tee /usr/share/keyrings/hashicorp-archive-keyring.gpg > /dev/null
    gpg --no-default-keyring \
    --keyring /usr/share/keyrings/hashicorp-archive-keyring.gpg \
    --fingerprint
    echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] \
    https://apt.releases.hashicorp.com $(lsb_release -cs) main" | \
    sudo tee /etc/apt/sources.list.d/hashicorp.list
    sudo apt update
    sudo apt-get install terraform
    terraform --version
   ```

3. **Git and GitHub CLI:**
   ```bash
   sudo apt install git -y
    sudo apt install gh -y
    git --version
    gh --version
   ```

4. **Nginx:**
   ```bash
   sudo apt install nginx -y
    sudo systemctl status nginx
   ```

5. **AWS CLI:**
   ```bash
   curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
   sudo ./aws/install --bin-dir /usr/local/bin --install-dir /usr/local/aws-cli --update
   aws --version
   ```

---

## Screenshots


### Creating VM Step 1
![Creating VM Step 1](https://github.com/Ainkkrader/DevOps-Task0/blob/main/crvmsp1.PNG)

### Creating VM Step 2
![Creating VM Step 2](https://github.com/Ainkkrader/DevOps-Task0/blob/main/crvmsp2.PNG)

### Creating VM Step 3
![Creating VM Step 3](https://github.com/Ainkkrader/DevOps-Task0/blob/main/crvmsp3.PNG)

### Creating VM Step 4
![Creating VM Step 4](https://github.com/Ainkkrader/DevOps-Task0/blob/main/crvm4.PNG)

### Version Docker
![Version Docker](https://github.com/Ainkkrader/DevOps-Task0/blob/main/docker.PNG)

### Version Docker Compose
![Version Docker Compose](https://github.com/Ainkkrader/DevOps-Task0/blob/main/docker%20compose.PNG)

### Version Git
![Version Git](https://github.com/Ainkkrader/DevOps-Task0/blob/main/git.PNG)

### Version Git CLI
![Version Git CLI](https://github.com/Ainkkrader/DevOps-Task0/blob/main/docker%20compose.PNG)

### Version Nginx
![Version Nginx](https://github.com/Ainkkrader/DevOps-Task0/blob/main/nginx.PNG)

### Version AWS 
![Version AWS](https://github.com/Ainkkrader/DevOps-Task0/blob/main/aws.PNG)

### Version Terraform 
![Version Terraform](https://github.com/Ainkkrader/DevOps-Task0/blob/main/terraform-version.PNG)

---


