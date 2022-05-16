Docker
=========

A role to install Docker

Requirements
------------

- `become: yes`
- `gather_facts: yes` if you don't specify `generic_docker_compose_os` and `generic_docker_compose_arch`

Role Variables
--------------

For all variables please see `defaults/main.yml`.


Dependencies
------------

None

Example Playbook
----------------

    ---
    - hosts: all
      gather_facts: yes
      become: yes
      roles:
        - generic_docker_role

[examples/deploy-docker.yml](examples/deploy-docker.yml)