Role Name
=========

Ansible role to install HUGO on Linux.

Requirements
------------

None

Role Variables
--------------
```yaml
hugo_version: 0.155.2
```
Hugo version to install

```yaml
hugo_arch: amd64
```
Hugo architecture, choices are: arm, arm64 and amd64.

```yaml
hugo_install_dir: /usr/local/bin
```
The directory where to install HUGO

```yaml
hugo_repo_url: https://github.com/gohugoio/hugo
```
URL of HUGO GitHub repository.

Dependencies
------------

None

Example Playbook
----------------

    - hosts: all
      roles:
         - role: egdoc.hugo

License
-------

GPLv2

Author Information
------------------

Written by Egidio Docile.
