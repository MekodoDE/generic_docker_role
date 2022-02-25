Docker
=========

A role to install Docker

Requirements
------------

- `become: yes`
- `gather_facts: yes`

Role Variables
--------------

For all variables please see `defaults/main.yml`.

    generic_docker_package: "docker-ce"
Change between docker-ce (Community Edition) and docker-ee (Enterprise Edition).

    generic_docker_daemon_json: {}
Add the content of the daemon.json if needed.

    generic_docker_pip_modules:
    - docker
Add more pip modules if needed.

    generic_docker_install_compose: true
Change this value to true if you don't need docker compose

    generic_docker_compose_version: "1.29.0"
Docker compose version



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