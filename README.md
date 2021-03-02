Fish Shell Role
================
<p align="right">
  <a href="https://github.com/namiops/fish_shell">
  <img alt="Build" src="https://github.com/namiops/fish_shell/actions/workflows/build.yml/badge.svg">
  <img alt="Issue" src="https://img.shields.io/github/license/namiops/fish_shell">
  <img alt="Issue" src="https://img.shields.io/github/issues/namiops/fish_shell">
  <img alt="Forfs" src="https://img.shields.io/github/forks/namiops/fish_shell">
  <img alt="Stars" src="https://img.shields.io/github/stars/namiops/fish_shell"> 
  </a>
</p>


Ansible Role for install fish shell to multi OS

Installation
------------
1. Install role with Ansible Galaxy

   ```
   ansible-galaxy install namiops.fish_shell
   ```
2. Then use the role in playbook:

   ```yaml
   - hosts: all
     roles:
       - fish_shell
   ```
3. Run with playbook

   ```shell script
   ansible-playbook playbook.yml -i inventory
   ```

Role Variables
-------------

* common_packages: []
* fish_as_default_shell: bool

Supporting OS
-------------
* CentOS 8, CentOs 7
* Debian 10, Debian 9
* Ubuntu 20.10, Ubuntu 20.04, Ubuntu 18.04

Working with this Role
======================
We welcome you to use Github to contribute and report bugs or suggest features.

Requirements
------------
To develop this role, you need some tools installed:
* [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) (latest)
* [Molecule](https://molecule.readthedocs.io/en/latest/index.html)
* Docker

Run full tests with molecule
===========================
This Role develop base on the tests with multiple docker instances with Molecule. To run full test with all docker images, just run:
```shell script
molecule test
```


Contributing with Pull Request
------------------------------
Before starting a pull request, please ensure that:

1. You open an issue first to discuss before you work on it, we don't want your time to be wasted.
2. You are working against the latest source on the *develop* branch.
3. You check existing [open](ht``tps://github.com/namiops/fish_shell/pulls) and [merged](https://github.com/namiops/fish_shell/pulls?q=is%3Apr+is%3Aclosed) pull requests to make sure someone else didn't solve the issue before you.

Then, for create a pull request:
1. Fork the repository.
2. Modify the source.
3. Ensure you ran the tests pass.
4. Commit to your fork.
5. Send us a pull request, check CI report, answer the questions and discuss in the Pull Request
6. Please keep engage to the conversation for your Pull Request merged

Authors Information
------------------
This Role develop by [namiops](https://github.com/namiops)

License
-------
- MIT
- Apache-2-0

