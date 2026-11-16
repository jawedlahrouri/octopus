[![Academic Year](https://img.shields.io/badge/Epitech-Tek2-green?style=for-the-badge&logo=epitech&logoColor=white)](https://www.epitech.eu/)

# Octopus Project (B-DOP-400)

This repository contains the Ansible infrastructure for the Octopus project.

## Structure
- `production`: Inventory file for the 5 target VMs.
- `playbook.yml`: Main playbook to orchestrate the deployment.
- `roles/`: Ansible roles for each component (Poll, Redis, Worker, Postgres, Result).
- `group_vars/`: Global and group-specific variables.
- `*.tar`: Application source code archives.

## Usage
1. Activate the environment:
   ```bash
   source venv/bin/activate
   ```
2. Run the playbook:
   ```bash
   ansible-playbook -i production playbook.yml
   ```
