
**Useful Ansible Commands**

*Run a playbook*

`$ ansible-playbook <playbook-location>/<play-book>.yml `

*Run a playbook for specific tag*

`$ ansible-playbook <playbook-location>/<play-book>.yml --tags <tag name>`

*Run a playbook which access encrypted secrets*

`$ ansible-playbook playbooks/setup-app.yml --ask-vault-pass`

*Command to see meta data of a host/inventory group*

`$ ansible -m setup app1`

*Execute an adhoc command on a host*

`$ ansible -m service -a "name=<service name> state=<service state>" --become <host group>`

*Create default file structure for roles using ansible galaxy*

`$ ansible-galaxy init <folder location>`

*Using Ansible Vault for secrets*

*create secrets file*

`$ ansible-vault create vars/secret-variables.yml`

*edit secrets file*

`$ ansible-vault edit vars/secret-variables.yml`