# Windows Ansible Roles

[![License: GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)](https://www.gnu.org/licenses/gpl-3.0)

Ansible roles for Windows configuration.

## Quick Intro

To install this collection from GitHub:

```
ansible-galaxy collection install git+https://github.com/myllynen/windows-ansible-roles,master
```

Depending on the environment and requirements separate playbooks and/or
vars files, group vars, variables defined in an inventory, or some other
approach might be appropriate for providing configuration variables for
the roles.

See the READMEs of [each role](roles) for descriptions of the parameters
they support.

See the example playbook [configure_windows.yml](configure_windows.yml)
for all the configuration options these roles support and how they could
be used together.

These roles have been tested with updated Windows Server 2019/2022/2025
using Ansible 2.14 - 2.19. READMEs of roles will list supported versions
where needed, by default all roles support all those Windows versions.

The roles will gather the minimum set of facts as needed meaning that
they can be used in setups where fact gathering is disabled.

This collection provides roles for automatically setting up OpenSSH SSH
Server (sshd) and WinRM remote access on recent Windows Server versions.
For a full description of WinRM configuration alternatives, see the
upstream
[Windows Remote Management for Ansible](https://docs.ansible.com/ansible/latest/user_guide/windows_winrm.html)
guide.

For Ansible Windows Guides, see:  
[https://docs.ansible.com/ansible/latest/user_guide/windows.html](https://docs.ansible.com/ansible/latest/user_guide/windows.html)

For available Ansible collections for Windows, see:  
[https://docs.ansible.com/ansible/latest/collections/ansible/windows/](https://docs.ansible.com/ansible/latest/collections/ansible/windows/)  
[https://docs.ansible.com/ansible/latest/collections/community/windows/](https://docs.ansible.com/ansible/latest/collections/community/windows/)

## See Also

See also
[https://github.com/myllynen/ansible-packer](https://github.com/myllynen/ansible-packer).

See also
[https://github.com/myllynen/rhel-ansible-roles](https://github.com/myllynen/rhel-ansible-roles).

## License

GPLv3+
