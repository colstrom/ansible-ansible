# ansible-ansible

Ansible is Simple IT Automation

[![Platforms](http://img.shields.io/badge/platforms-ubuntu-lightgrey.svg?style=flat)](#)

## Tunables

* `ansible_forks_default` (integer) - Number of concurrent requests Ansible can make
* `ansible_host_key_checking_default` (boolean) - Check SSH Host Keys?
* `ansible_privilege_escalation_default` (boolean) - Should playbooks try to become a privileged user by default?

## Dependencies

* [colstrom.apt-repository](https://github.com/colstrom/ansible-apt-repository/)

## Example Playbook
    - hosts: servers
      roles:
       - role: colstrom.ansible
         ansible_host_key_checking_default: no
         ansible_privilege_escalation_default: yes

## License

[MIT](https://tldrlegal.com/license/mit-license)

## Contributors
  * [Chris Olstrom](https://colstrom.github.io/) | [e-mail](mailto:chris@olstrom.com) | [Twitter](https://twitter.com/ChrisOlstrom)
  * Royston Tong
  * Aaron Pederson
