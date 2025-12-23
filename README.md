# System-packages-Role

[![Alma9-CI](https://github.com/philnewm/ansible-system-packages/actions/workflows/alma9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-system-packages/actions/workflows/alma9-ci-caller.yml) [![Rocky9-CI](https://github.com/philnewm/ansible-system-packages/actions/workflows/rocky9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-system-packages/actions/workflows/rocky9-ci-caller.yml) [![CentOSStream9-CI](https://github.com/philnewm/ansible-system-packages/actions/workflows/centosstream9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-system-packages/actions/workflows/centosstream9-ci-caller.yml) [![Fedora43-CI](https://github.com/philnewm/ansible-system-packages/actions/workflows/fedora43-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-system-packages/actions/workflows/fedora43-ci-caller.yml)<br>
[![Ubuntu2404-CI](https://github.com/philnewm/ansible-system-packages/actions/workflows/ubuntu2404-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-system-packages/actions/workflows/ubuntu2404-ci-caller.yml) [![Debian13-CI](https://github.com/philnewm/ansible-system-packages/actions/workflows/debian13-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-system-packages/actions/workflows/debian13-ci-caller.yml)

Role description

This role includes a molecule testing setup as a submodule at `molecule/`

## Structure

```code
📦 ansible-system-packages
 ┣ 📂defaults
 ┃ ┗ 📜main.yml
 ┣ 📂files
 ┃ ┣ 📜packages_list.yml
 ┃ ┗ 📜repo_list.yml
 ┣ 📂meta
 ┃ ┗ 📜main.yml
 ┣ 📂 molecule
 ┃ ┗ 📂 default
 ┃   ┗ 📜, 📜, 📜, scenario_files
 ┣ 📂tasks
 ┃ ┣ 📜absent.yml
 ┃ ┣ 📜debian_repos.yml
 ┃ ┣ 📜main.yml
 ┃ ┣ 📜present.yml
 ┃ ┣ 📜redhat_repos.yml
 ┃ ┗ 📜tests.yml
 ┣ 📂vars
 ┃ ┗ 📜main.yml
 ┣ 📜.gitignore
 ┣ 📜.gitmodules
 ┗ 📜README.md

```

Describe and explain role structure.

## Requirements

Elaborate external dependencies and how to use them.

## Role Variables

* defaults/main.yml
  * first_var
  * sec_var
  * third_var
* vars/main.yml
  * first_var
  * sec_var
  * third_var

## Dependencies

List role ansible-galaxy dependencies - if any.

## Example Playbook

Add an example playbook

```yaml
---

tasks:
  - name: Include ansible-system-packages present
    ansible.builtin.include_role:
      name: ansible-system-packages
    vars:
      state: present

...
```

## License

Add license - if any.
