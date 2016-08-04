# ansible-role-osticket

[![Build Status](https://travis-ci.org/linuxhq/ansible-role-osticket.svg?branch=master)](https://travis-ci.org/linuxhq/ansible-role-osticket)

RHEL/CentOS - Support Ticket System

## Requirements

None

## Role Variables

Available variables are listed below, along with default values:

    osticket_httpd_customlog: osticket-access_log
    osticket_httpd_documentroot: /usr/share/osTicket/htdocs/
    osticket_httpd_errorlog: osticket-error_log
    osticket_httpd_servername: osticket
    osticket_pipe: helpdesk

Additional variables available, not defined by default:

    osticket_httpd_serveralias: []

## Dependencies

 * https://galaxy.ansible.com/linuxhq/epel/
 * https://galaxy.ansible.com/linuxhq/linuxhq/

## Example Playbook

    - hosts: servers
      roles:
        - role: linuxhq.osticket
          osticket_httpd_serveralias:
            - helpdesk.linuxhq.org

## Partners

[![packagecloud](http://dka575ofm4ao0.cloudfront.net/pages-transactional_logos/retina/10543/gKme3F4XRaC5EyKJzKsA)](https://packagecloud.io)

Do you need trustworthy hosted package repositories?  Then packagecloud is for you.

A big thank you to packagecloud for supporting the open source community!

## License

BSD

## Author Information

This role was created by [Taylor Kimball](http://www.linuxhq.org).
