Role Name
=========

mailcow Mailserver and Groupware

- https://github.com/mailcow/mailcow-dockerized
- https://mailcow.github.io/mailcow-dockerized-docs/
- https://mailcow.email/
- https://www.servercow.de/mailcow

Requirements
------------

- Debian 9 stretch
- 1.5 to 2 GB RAM

### Info

- mailcow: dockerized requires some ports to be open for incoming connections, so make sure that your firewall is not blocking these.
- Make sure that no other application is interferring with mailcow's configuration, such as another mail service
- A correct DNS setup is crucial to every good mailserver setup, so please make sure you got at least the basics covered before you begin!
- Make sure that your system has a correct date and time setup. This is crucial for stuff like two factor TOTP authentication.

https://mailcow.github.io/mailcow-dockerized-docs/prerequesite-system/


Role Variables
--------------

Set your Server IP, Fully Qualified Domain Name and Timezone in defaults/main.yml


Example Playbook
----------------

    - hosts: servers
      roles:
         - chriswayg.mailcow

`$ ansible-playbook -i hosts -v -u root mailcow.yml`

License
-------

BSD

Author Information
------------------

Christian Wanger
