hxpro.pebble
===============

A miniature version of Boulder, Pebble is a small ACME-12 test server not suited for use as a production CA.

Role Variables
--------------
```
go_path: "$HOME/go"
```

Dependencies
------------

 - hxpro.bootstrap

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: hxpro.pebble
           go_path: /opt/go

License
-------

WTFPL

Author Information
------------------

Matěj Koudelka <matej@hxpro.cz>
