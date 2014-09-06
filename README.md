openwrt-wireless
================

wireless config of your openwrt system.
compare: [http://wiki.openwrt.org/doc/uci/wireless]

Role Variables
--------------

a bunch of per interface settings are all nested in a single dict
`wireless`. the layout is a bit weird because i use with_subelements.
look at the defaults and tasks directory. if you have a suggestion for
how to do it more effectively without duplication, let me know!

you may want to consider `hash_behaviour=merge` in your ansible.cfg

Dependencies
------------

[lefant.openwrt-uci]

Example Playbook
----------------

[https://github.com/lefant/ansible-openwrt/blob/master/openwrt.yml]

Requirements
------------

must be kept minimal as this is supposed to run on openwrt embedded
systems. in particular we try get by with plain POSIX shell, using
neither python nor bash in any way. lua could be an option as that
seems to be the openwrt scripting language of choice.

License
-------

BSD

Author Information
------------------

Fabian Linzberger, [http://e.lefant.net/]



[https://github.com/lefant/ansible-openwrt/blob/master/openwrt.yml]: https://github.com/lefant/ansible-openwrt/blob/master/openwrt.yml
[http://wiki.openwrt.org/doc/uci/wireless]: http://wiki.openwrt.org/doc/uci/wireless
[lefant.openwrt-uci]: https://galaxy.ansible.com/list#/roles/1645
[http://e.lefant.net/]: http://e.lefant.net/
