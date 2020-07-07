ssmtp
=========

Installs and configures a nullmailer (ssmtp).

Requirements
------------

Debian or Ubuntu.

Role Variables
--------------

ssmtp_mailname: Name of the server (NOT the From in the email!), defaults to ansible_fqdn
ssmtp_mailhub: Relay server name, defaults to smtp.eu.mailgun.org
ssmtp_hostname: Server's FQDN. Defaults to ansible_fqdn
ssmtp_port: Server port. 
ssmtp_rewritedomain:  Defaults to ansible_domain
ssmtp_root: Defaults to system_emailaddres

Example Playbook
----------------

    - hosts:
        servers:
          ssmtp_mailhub: "smtp.eu.mailgun.org"
          ssmtp_port: 587
          ssmtp_rewritedomain: "www.example.com"
      roles:
         - ssmtp
