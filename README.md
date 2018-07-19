# ansible_network_backup
Playbook for network backup with Ansible

It will create an folder (default ./CFGS/ < hostname >/ and place current (latest) config file in there.
When by new run of playbook there are changes with latest config, the old config will be placed in /history/<date>_<time>_hostname.conf

Variables needed
----------------
There is one variable needed "platform"  where the platform type is defined, this is needed for selection of the right module

NAPALM Module preferred

Supported:
* cisco_ios (CLI and NAPALM)
* cisco_nxos (CLI and NAPALM)
* alcatel (NAPALM) < ToDo


Cisco IOS
-------


