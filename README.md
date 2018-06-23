# ansible-role-osticket

[![Build Status](https://travis-ci.org/linuxhq/ansible-role-osticket.svg?branch=master)](https://travis-ci.org/linuxhq/ansible-role-osticket)
[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-osticket-blue.svg?style=flat)](https://galaxy.ansible.com/linuxhq/osticket)
[![License](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](COPYING)

RHEL/CentOS - Support Ticket System

## Requirements

None

## Role Variables

Available variables are listed below, along with default values:

    osticket_customlog: osticket-access_log
    osticket_documentroot: /usr/share/osticket/htdocs/
    osticket_errorlog: osticket-error_log
    osticket_pipe: helpdesk
    osticket_serveralias: []
    osticket_servername: osticket

## Dependencies

 * https://galaxy.ansible.com/linuxhq/linuxhq/

## Example Playbook

    - hosts: servers
      roles:
        - role: linuxhq.osticket
          osticket_httpd_serveralias:
            - helpdesk.linuxhq.org

## License

Copyright (C) 2018 Taylor Kimball <tkimball@linuxhq.org>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.
