# Ansible Apache Setup

This repository contains an Ansible playbook to install and configure Apache on a server. It uses Ansible roles to organize tasks and configurations and includes error handling.

## Prerequisites

- Ansible installed on your local machine.
- Access to the server (e.g., a VM) with SSH credentials.
- A configured inventory file with your server details.

## Directory Structure

- `roles/` - Contains roles for Apache and common tasks.
- `inventory` - Contains the server IP addresses.
- `playbook.yml` - Main Ansible playbook.
- `README.md` - This file.

## Setup

1. **Update Inventory File**: Modify the `inventory` file to include your server's IP address and SSH user.

2. **Run the Playbook**:

   ```bash
   ansible-playbook -i inventory playbook.yml --ask-become-pass