Configure some basics on your Debian/Ubuntu system.
- Replaces /etc/motd. 
- Configure the shell prompt (PS1) to be colorful.
- Removes cloud-init 

Requirements
------------

None.

Role Variables
--------------

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - basics_debian

Author Information
------------------

