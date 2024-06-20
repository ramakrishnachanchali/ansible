# Running Ansible Playbook with Specific Roles and Tags

## Overview

This guide explains how to run an Ansible playbook that executes specific roles using tags. Tags are useful for running specific parts of your playbook without executing the entire playbook.

## Prerequisites

- Ansible installed on your control node.
- An inventory file (`inventory.ini`) that lists your target hosts.
- A playbook file (`roles.yaml`) that defines the roles and tasks.
- Properly configured roles in your Ansible directory structure.

## Example Command

To execute the playbook with a specific tag, use the following command:

```bash
ansible-playbook roles.yaml -i ../inventory.ini --tags=httpd
