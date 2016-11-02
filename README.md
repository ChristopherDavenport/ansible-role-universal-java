Universal Java Jdk Installer
=========

This is intended to install a jdk on almost any system.

### Requirements
------------

None

Role Variables
--------------

Options are Open or Oracle

```
java_type: Open
```

Options are 7 or 8 for Oracle and 7, 8 or 9 for Open

```
java_version: "8"
```

Temporary Storage Location

```
java_tmp_storage: /tmp/java_install
```


Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
    - hosts: servers
      roles:
         - ChristopherDavenport.universal-java
```

License
-------

MIT

Author Information
------------------

This role was created in 2016 by ChristopherDavenport.
