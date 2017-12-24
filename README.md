Video4Linux (V4L)
=========

Install desired version of V4L.

Requirements
------------

Refer to the V4L documentation.

Role Variables
--------------

Required variable: `v4l_src`
Example: `v4l_src: http://launchpadlibrarian.net/235110130/v4l-utils_1.10.0-1_amd64.deb`

Dependencies
------------

N/A

Example Playbook
----------------
```
$ ansible-galaxy install stockhausenj.magewell
$ ansible-playbook -i inventory.yaml install-v4l.yaml -u <ssh-user> -K
```
```
- hosts: all
  roles:
    - include_role:
        name: stockhausenj.video4linux
      vars:
        v4l_src: http://launchpadlibrarian.net/235110130/v4l-utils_1.10.0-1_amd64.deb
```

License
-------

MIT
