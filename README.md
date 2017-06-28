# Ansible role for fail2ban


Setup fail2ban.

## Requirements

- Debian
- Ubuntu

## Role Variables

see defaults/main.yml

## Dependencies

None.

## Example Playbook

Example:

    - hosts: servers
      become: yes
      roles:
         - role: znz.fail2ban

Another example:

    - hosts: all
      become: yes
      roles:
      - role: znz.fail2ban
        fail2ban_files:
        - local-apache.conf

## License

MIT License
