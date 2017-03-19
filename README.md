# Ansible Role: rsyslog

Installs [rsyslog](http://www.rsyslog.com/) on Debian/Ubuntu and configures itself as a centralized logging service (One server/master, any number of clients).

## Role Variables

    rsyslog_master: 127.0.0.1

The IP Address of the master/rsyslog server

## Dependencies

None.

## Example Playbook (Server/Master)

    - hosts: all
      roles:
        - { role: pabloguerino.rsyslog, type: server }

## Example Playbook (Client)

    - hosts: all
      roles:
        - { role: pabloguerino.rsyslog, type: client }

## License

MIT / BSD

## Author Information

This role was created in 2016 by [Pablo Guerino](https://github.com/pabloguerino)