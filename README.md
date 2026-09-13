# Ansible Deployment: adguard

[![Ansible Lint](https://github.com/leberkaslabs/ansible-adguard-deployment/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/leberkaslabs/ansible-adguard-deployment/actions/workflows/ansible-lint.yml)

Ansible playbooks for deploying AdGuard Home.

## Prerequisites

- Ensure you have Ansible installed (e.g. `pip3 install ansible`)
- **Development**: Install the pip packages listed in [requirements.txt](requirements.txt)

## Usage

> [!NOTE]
> Before running the playbooks, prepare the inventory and configuration files.

1. Copy the example inventory file to `hosts.yml`:

    ```bash
    cp inventories/hosts.example.yml inventories/hosts.yml
    ```

2. Run the Ansible playbook:

    ```bash
    ansible-playbook main.yml
    ```

## Development

This project includes [Ansible Molecule](https://github.com/ansible/molecule) to streamline testing and development.

```bash
# Run the Vagrant scenario explicitly
molecule test
```

Molecule will automatically create, converge, verify and destroy the test instances.

## License

Copyright (c) 2026 Niclas Spreng
