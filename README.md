# ansible_role_template
Template for Ansible roles

```
postfix__inet_interfaces: "127.0.0.1, ::1"

postfix__inet_interfaces: "127.0.0.1, ::1, {{ hostvars[ inventory_hostname ].ansible_default_ipv4.address }}, {{ hostvars[ inventory_hostname ].ansible_default_ipv6.address }}"

 Testing
----------
This role is tested with [these github-action](https://github.com/search?q=topic%3Acheck-ansible+topic%3Agithub-actions+org%3Aroles-ansible&type=Repositories) tests for different versions of differen linux systems. Linting is tested via travis-ci and the  [ansible-lint action](https://github.com/marketplace/actions/ansible-lint).
If you want to find out more about our tests, please have a look at the github marketplace.

| test status | Github Marketplace |
| :---------  | :----------------  |
| [![Ansible Lint check](https://github.com/roles-ansible/ansible_role_template/workflows/Ansible%20Lint%20check/badge.svg)](https://github.com/roles-ansible/ansible_role_template/actions?query=workflow%3A%22Ansible+Lint+check%22) | [ansible-lint action](https://github.com/marketplace/actions/ansible-lint)
| [![Ansible check debian:stable](https://github.com/roles-ansible/ansible_role_template/workflows/Ansible%20check%20debian:stable/badge.svg)](https://github.com/roles-ansible/ansible_role_template/actions?query=workflow%3A%22Ansible+check+debian%3Astable%22) | [ansible test with debian stable](https://github.com/marketplace/actions/check-ansible-debian-stable) |
| [![Ansible check debian:latest](https://github.com/roles-ansible/ansible_role_template/workflows/Ansible%20check%20debian:latest/badge.svg)](https://github.com/roles-ansible/ansible_role_template/actions?query=workflow%3A%22Ansible+check+debian%3Alatest%22) | [ansible test with debian latest](https://github.com/marketplace/actions/check-ansible-debian-latest) |
| [![Ansible check debian:sid](https://github.com/roles-ansible/ansible_role_template/workflows/Ansible%20check%20debian:sid/badge.svg)](https://github.com/roles-ansible/ansible_role_template/actions?query=workflow%3A%22Ansible+check+debian%3Asid%22) | [ansible test with debian sid](https://github.com/marketplace/actions/check-ansible-debian-sid) |
| [![Ansible check debian:buster](https://github.com/roles-ansible/ansible_role_template/workflows/Ansible%20check%20debian:buster/badge.svg)](https://github.com/roles-ansible/ansible_role_template/actions?query=workflow%3A%22Ansible+check+debian%3Abuster%22) | [ansible test with debian buster](https://github.com/marketplace/actions/check-ansible-debian-buster) |
| [![Ansible check debian:stretch](https://github.com/roles-ansible/ansible_role_template/workflows/Ansible%20check%20debian:stretch/badge.svg)](https://github.com/roles-ansible/ansible_role_template/actions?query=workflow%3A%22Ansible+check+debian%3Astretch%22) | [ansible test with debian stretch](https://github.com/marketplace/actions/check-ansible-debian-stretch) |
| | |
| [![Ansible check ubuntu:latest](https://github.com/roles-ansible/ansible_role_template/workflows/Ansible%20check%20ubuntu:latest/badge.svg)](https://github.com/roles-ansible/ansible_role_template/actions?query=workflow%3A%22Ansible+check+ubuntu%3Alatest%22) | [ansible test with ubuntu latest](https://github.com/marketplace/actions/check-ansible-ubuntu-latest) |
| [![Ansible check ubuntu:bionic](https://github.com/roles-ansible/ansible_role_template/workflows/Ansible%20check%20ubuntu:bionic/badge.svg)](https://github.com/roles-ansible/ansible_role_template/actions?query=workflow%3A%22Ansible+check+ubuntu%3Abionic%22) | [ansible test with ubuntu bionic](https://github.com/marketplace/actions/check-ansible-ubuntu-bionic) |
| [![Ansible check ubuntu:trusty](https://github.com/roles-ansible/ansible_role_template/workflows/Ansible%20check%20ubuntu:trusty/badge.svg)](https://github.com/roles-ansible/ansible_role_template/actions?query=workflow%3A%22Ansible+check+ubuntu%3Atrusty%22) | [ansible test with ubuntu trusty](https://github.com/marketplace/actions/check-ansible-ubuntu-trusty) |
