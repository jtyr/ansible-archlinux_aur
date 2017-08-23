archlinux_aur
=============

Ansible role which installs Arch Linux packages from AUR.


Examples
--------

```yaml
---

- name: Install Yaourt
  hosts: all
  vars:
    archlinux_aur_pkgs:
      - package-query
      - yaourt
  roles:
    - archlinux_aur
```


Role variables
--------------

Variables used by the role is as follows:

```yaml
# Packages to be installed
archlinux_aur_pkgs: []

# Force the installation even if the packages are already installed
archlinux_aur_force: false

# Under which user to build the packages
archlinux_aur_user: nobody
```


License
-------

MIT


Author
------

Jiri Tyr
