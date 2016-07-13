ZendServer
Ansible role to install Zend Server with Apache/Nginx on Ubuntu/Centos

Role Variables
--------------

At the moment, you can specify the following variables:

| Name               | Default |Description                                         |             | 
|--------------------|---------|----------------------------------------------------|-------------|
| web_server         | apache  | The version of Zend Server to install              |apache/nginx |
| zendserver_version | 8.5     | The version of PHP to install                      |8.0, 8.5, 9.0|
| php_version        | 5.6     | Add the Zend Server binary dir to the bash profile |5.6, 7.0     |


Examples
--------
```
---
- name: Zend Server 
  hosts: all
  roles:
    - { role: Uccio.ZendServer, php_version: 5.6, zendserver_version: 8.5.4 }
```


Dependencies
------------
None

Author Information
------------------

Created by Uccio
http://uccio.org
