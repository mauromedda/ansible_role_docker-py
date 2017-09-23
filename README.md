mauromedda.ansible_role_dockerpy
=================================

Install docker-py on the CentOS distribution.

## Requirements

No.

## Role Variables

Available variables are listed below, along with default values (see [`defaults/main.yml`](defaults/main.yml)):

    dockerpy_version

The docker-py version to install. Default is empty.

## Dependencies

None.

## Example

$ ansible-galaxy install mauromedda.ansible_role_dockerpy

$ cat > site.yml <<-EOF
- hosts: localhost
  become: true
  connection: local

  roles:
    - { role: mauromedda.ansible_role_epel }
    - { role: mauromedda.ansible_role_docker }
    - { role: mauromedda.ansible_role_dockerpy }
EOF

$ ansible-playbook site.yml

## License

BSD

## Author Information

Mauro Medda
