Vector
=========

This role installs and configures the vector.

Role Variables
--------------

_vector_version_ - needed vector version </br>
_vector_data_dir_ - where must be data directory, default "/var/lib/vector" </br>
_clickhouse_host_ - ip or fqdn of the clickhouse node </br>
_clickhouse_user_ - user with access to clickhouse </br>
_clickhouse_password_ - user password </br>

Example Playbook
----------------

You can use this role simple like this:

    - hosts: servers
      roles:
         - { role: vector, clickhouse_host: 127.0.0.1 }

License
-------

MIT

Author Information
------------------

Nikolay Mokrov
