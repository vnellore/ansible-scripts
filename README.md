
**Useful Ansible Commands**

*Run a playbook*

`$ ansible-playbook <playbook-location>/<play-book>.yml `

*Command to see meta data of a host/inventory group*

`$ ansible -m setup app1`

*Execute an adhoc command on a host*

`$ ansible -m service -a "name=<service name> state=<service state>" --become <host group>`

*Create default file structure for roles using ansible galaxy*

`$ ansible-galaxy init <folder location>`