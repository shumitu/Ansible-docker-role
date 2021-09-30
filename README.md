Basic ansible docker role
=========

Simple ansible role created to deploy docker on various linux distributions.
This role installs docker with required dependencies and starts docker service afterwards.

Supported Linux distributions
------------

This role has been tested on:
- CentOS 7
- CentOS 8
- RHEL 7
- RHEL 8
- Ubuntu 18 - Bionic 
- Ubuntu 20 - Focal
- Ubuntu 21 - Hirsute
- Debian 11 - Bullseye
- Debian 10 - Buster
- Fedora 33
- Fedora 34

Role Variables
--------------

Distribution dependent variables are placed in corresponding files inside "vars" directory.
They include links to docker repositories and GPG keys.

Example Playbook
----------------

Example playbook used to run above role is presented below.
```yaml
- name: Run docker role
  hosts: all
  roles:
    - role: docker
```

License
-------

BSD

Author Information
------------------

Sergiusz Parchatko  
sergiusz.parchatko@gmail.com  
https://github.com/shumitu  

