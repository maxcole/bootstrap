# Bootstrap

Bootstrap script for home lab infrastructure setup.

## Overview

This script automates the initial setup of an rws bootstrap machine (e.g., Raspberry Pi) by installing Ansible, creating an Ansible eser, and installing an Ansible collection.

## Requirements

- sudo is already installed
- The current user has sudo permissions
- Internet connectivity
- SSH key access to GitHub repositories

## What it does

### Bootstrap Script (`bootstrap.sh`)

1. Installs the OS Ansible package
2. Creates a user with an authorized_keys file and passwordless sudo
3. Clones the rjayroach.common Ansible collection repo and assigns ownership to the Ansible user

## Usage

```bash
curl -sSL https://raw.githubusercontent.com/maxcole/rws-bootstrap/refs/heads/main/bootstrap.sh | bash -s -- -icu ansible
```

## Files

- `bootstrap.sh` - Main bootstrap script
