# ansible-volatility
This role is for use by DFIR/security options teams to quickly deploy and manage a Linux system to be used for memory forensics using the [Volatility Framework](http://www.volatilityfoundation.org/).

##Role Variables
```yaml
users: []
```

##Example Playbook
Assuming you have a single host or set of hosts you use for this purpose, and that you include the variable "forensics" in either the host_vars or group_vars files as appropriate, the following playbook would deploy this role.

```yaml
    - hosts: all
      become: true

      roles:
         - { role: ansible-volatility, when: forensics }
```

##License
MIT

##Author Information
Matt Shepherd aka matts-mpg
Vice President at MindPoint Group