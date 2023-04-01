# Ansible Role: SteamCMD

[![Molecule CI](https://github.com/8kbmemories/steamcmd-ansible/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/8kbmemories/steamcmd-ansible/actions/workflows/ci.yml)

This Ansible role installs [SteamCMD](https://developer.valvesoftware.com/wiki/SteamCMD) on a target system and optionally creates a user to run it with limited privileges.

Steamcmd is a command-line version of the Steam client which can be used to install and update various dedicated servers including games like Counter-Strike and Team Fortress 2.

# Requirements
This role requires Ansible 2.4 or higher and is designed to work with the following operating systems:

- Debian 10/11
- Ubuntu 18.04/20.04
# Role Variables
The following variables can be set to customize the behavior of this role:

- `steamcmd_account_name` (default: `steam`): The username of the user that will run SteamCMD.
- `steamcmd_create_account` (default: `true`): Specify if a unprivileged user needs to be created.
# Dependencies
This role has no dependencies.

# Example Playbook
Here is an example playbook that uses this role:

```yaml
- hosts: all
  roles:
    - 8kbmemories.steamcmd
```

# License
This role is licensed under the MIT License. See the LICENSE file for details.



