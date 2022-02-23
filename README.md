- [ansible-role-nfsclient](#ansible-role-nfsclient)
  - [Requirements](#requirements)
  - [Role Variables](#role-variables)
  - [Dependencies](#dependencies)
  - [Example Playbook](#example-playbook)
  - [License](#license)

# ansible-role-nfsclient

An [Ansible](https://www.ansible.com) role to install/configure an NFS Client

## Requirements

None

## Role Variables

```yaml
---
# defaults file for ansible-role-nfsclient
nfs_client_mounts: []
  # - mount:
  #   fstype: 'nfs'
  #   opts:
  #     - 'rsize=8192'
  #     - 'wsize=8192'
  #     - 'intr'
  #   path: '/opt/nfs/test1'
  #   src: '192.168.250.10:/opt/nfs/test1'
  #   state: 'mounted'
  # - mount:
  #   fstype: 'nfs'
  #   opts:
  #     - 'rsize=8192'
  #     - 'wsize=8192'
  #     - 'intr'
  #   path: '/opt/nfs/test2'
  #   src: '192.168.250.10:/opt/nfs/test2'
  #   state: 'mounted'
```

## Dependencies

None

## Example Playbook

```yaml
---
- hosts: nfs_client
  vars:
  roles:
    - role: ansible-role-nfsclient
  tasks:
```

## License

MIT

