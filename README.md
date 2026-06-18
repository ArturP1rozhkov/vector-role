## vector-role
This role installs and configures Vector 
### Requirements
- Ansible
- Linux host with access to download Vector archive
- User account with write access to the installation directory
### Role Variables
All variables that can be overridden are stored in `defaults/main.yml`.

| Name                 | Default Value   | Description                               |
| -------------------- | --------------- | ----------------------------------------- |
| `vector_version`     | `0.37.1`        | Version of Vector to install.             |
| `vector_install_dir` | `~/vector-role` | Directory where Vector will be installed. |

### Dependencies
No dependencies.
### Example Playbook
```yaml
- name: Install Vector
  hosts: vector
  roles:
    - role: /home/vboxuser/ansible/vector-role
```
### Notes
This role is adapted for the homework and installs Vector into the user home directory.
### License 
Not specified.
### Author Information Role author: 
Artur P1rozhkov