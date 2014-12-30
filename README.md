Role: cns.mailname
========

This role sets the visible mail name of the system. The  file /etc/mailname is a plain ASCII configuration file, which on a Debian system contains the visible mail name of the system.  It is used by many different programs, usually programs that wish to send or relay mail, and need to know the name of the system. The  file  contains only one line describing the fully qualified domain name that the program wishing to get the mail name should use (that is, everything after the @).

Requirements
------------

Nothing, it runs out of the box.

Role Variables
--------------

In the current version, you can specify the following variables:

| Name               | Default |                                      |
|--------------------|---------|--------------------------------------|
| mailname           |   ---   | The visible mail name of the system. |


Dependencies
------------

This package has no dependencies.

License
-------

GPLv2

Author Information
------------------

Created by Sam Morrison
https://www.twitter.com/samcns

Examples
--------

```yaml
---
- name: common role test
  hosts: all
  roles:
    - cns.mailname
```
