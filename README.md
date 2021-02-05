# jtprog.install_base_soft

![GitHub Workflow Status](https://img.shields.io/github/workflow/status/jtprog/ansible-role-install-base-soft/CI?label=CI) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/jtprog/ansible-role-install-base-soft/Release?label=Release) ![GitHub](https://img.shields.io/github/license/jtprog/ansible-role-install-base-soft)

Simple role for install base soft for comfort using remote server.


## Role Variables


See [`defaults/main.yml`](defaults/main.yml).


## Example Playbook

Example playbook:
```yaml
---
- name: Installing basic software
  hosts: all
  become: true

  vars:
    base_soft_list_extra:
      - ansible
      - net-tools
      - python3-pip
      - python3-setuptools
      - python3-wheel
      - ansible-lint
      - yamllint

  roles:
    - jtprog.install_base_soft
```

## License

See [LICENSE](LICENSE.md)
