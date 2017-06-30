freepbx13
===============

Updated role that will install Freepbx 13 on CentOS 7. This fork addresses several errors I encountered using the original role and adds TLS/SRTP support. It follows the basic installation described in the [official guide](https://wiki.freepbx.org/display/FOP/Installing+FreePBX+13+on+CentOS+7).  


Requirements
---------------------

Needs root/sudo

Role Varibles
-----------------

Nothing for now.

Example
---------------

    - hosts: freepbx
      user: root
      roles:
          - {role: dallen1.freepbx13}

Dependencies
-----------------

None

License
-------

2-clause BSD

My Information
-----------
Dustin Allen
[LinkedIn](https://www.linkedin.com/in/dustin-allen-b9277535/)

Original Author Information
------------------

Blagovest Petrov
http://petrovs.info


Notice
------

Tested on Centos 7 running on LXC. Should work on older versions too.

TODO
----
* Support for Debian/Ubuntu
