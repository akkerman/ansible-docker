ansible-docker
=========

Installs docker on ubuntu bionic with version pinning support.

Requirements
------------

None.

Role Variables
--------------

Role variables with their defaults:

```yaml
docker_version: "18.06.1"
docker_apt_key_id: 9DC858229FC7DD38854AE2D88D81803C0EBFCD88
docker_apt_key_url: https://download.docker.com/linux/ubuntu/gpg
```

The `docker_version` should be the version you want pinned, so a newer version does not automatically get installed when adding a server later.


Dependencies
------------

None

Example Playbook
----------------


```yaml
- hosts: all
    become: true
    roles:
        - ansible-docker
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a
website (HTML is not allowed).
