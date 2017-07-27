freepbx13
===============

Updated role that will install Freepbx 13 on CentOS 7. This fork addresses several errors I encountered using the original role and adds TLS/SRTP support. It follows the basic installation described in the [official guide](https://wiki.freepbx.org/display/FOP/Installing+FreePBX+13+on+CentOS+7).  


Requirements
---------------------

Needs root/sudo

Role Varibles
-----------------

Asterisk compilation options can be defined. The default options are to include chan_sip and format_mp3. For how to get the list of options check out this [Asterisk Page](https://wiki.asterisk.org/wiki/display/AST/Using+Menuselect+to+Select+Asterisk+Options)

WIP: Configurable FreePBX module installation from role.

Example
---------------

    - hosts: freepbx
      user: root
      roles:
          - role: dallen1.freepbx13
            asterisk_options:
              - chan_sip
              - format_mp3


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

Tested on CentOS 7 running on LXC. Probably won't work on older versions as they have differnt package requirements.

TODO
----
* Support for Debian/Ubuntu/CentOS 6
