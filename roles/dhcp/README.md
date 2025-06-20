Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

The following variables can be set to customize this role (see `defaults/main.yml` for structure and defaults):

- `dhcp_ctrl_agent_config`: Controls the Kea Control Agent configuration, including authentication, certificates, and control sockets.
- `dhcp_dhcp4_config`: Defines the Kea DHCPv4 server configuration, such as interfaces, lease database, timers, and subnets.
- `dhcp_ddns_config`: Sets the Kea DHCP DDNS (Dynamic DNS) configuration, including server address, protocol, and domain settings.

Override these variables in your playbook or inventory as needed.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
