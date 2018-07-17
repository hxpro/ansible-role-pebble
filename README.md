hxpro.pebble
===============

A miniature version of Boulder, Pebble is a small ACME-12 test server not suited for use as a production CA.

Role Variables
--------------
```
go_path: "$HOME/go"

pebble_listen: '0.0.0.0:14000'
pebble_certificate: '{{ go_path }}/src/github.com/letsencrypt/pebble/test/certs/localhost/cert.pem'
pebble_key: '{{ go_path }}/src/github.com/letsencrypt/pebble/test/certs/localhost/key.pem'
pebble_http_port: 80
pebble_tls_port: 443

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
