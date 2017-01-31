redshift Ansible role
=====================

Installs and enables the redshift system service
for controlling screen color temperature.

Requirements
------------

Assumes systemd for init system (due to the `--user` flag).

Role Variables
--------------

```yaml
redshift_packages:
  - redshift

# Whether systemd service is enabled to autostart.
redshift_service_enabled: yes
# Whether role should ensure service is running
redshift_service_state: started
# Whether `--user` flag is passed to systemd.
redshift_service_user: yes
```

Dependencies
------------

Example Playbook
----------------

```yaml
- hosts: workstations
  roles:
    - role: conorsch.redshift
```

License
-------

MIT
