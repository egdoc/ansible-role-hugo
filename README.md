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
hugo checksum: a680e2c6dd0e2244c237c85b549cb8697778cd068c84af1f7b0d9422827a554c
```
Checksum of the HUGO tarball. If you change HUGO version, you must also change this.

```yaml
hugo_tarball: hugo_{{ hugo_version }}_linux-{{ hugo_arch }}.tar.gz
```
This variable is used to construct the tarball name.

```yaml
hugo_download_dir: /tmp
```
Download location for the HUGO tarball

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
