Universal Java Jdk Installer
=========

[![Build Status](https://travis-ci.org/ChristopherDavenport/ansible-role-universal-java.svg?branch=master)](https://travis-ci.org/ChristopherDavenport/ansible-role-universal-java)

This is intended to install a jdk on almost any system.

Please notify me of any issues or

### Requirements
------------

None

Role Variables
--------------

Options are Open or Oracle

```yaml
java_type: Open
```

Options are 7 or 8 for Oracle and 7, 8 or 9 for Open

```yaml
java_version: "8"
```


Since JAVA_HOME is dependent on the operating system, this role effectively
puts it in place for almost all builds however as it is included dynamically
that means that it will not be able to be called from other roles.

If you want to set your own custom JAVA_HOME place the variable that is
not currently in the default file and assign it

```yaml
java_home: ${LOCATION_OF_CHOICE}
```


Whether Or Not To Install a script that will set JAVA_HOME environment
variable

```yaml
java_home_install_script: True
```

Name of the script that will be placed into /etc/profile.d/

```yaml
java_home_script_name: java_home.sh
```

Temporary Storage Location

```yaml
java_tmp_storage: /tmp/java_install
```


Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
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
