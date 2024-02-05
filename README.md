```
I've used letsencrypt to obtain fullchain.pem and privkey.pem files.
You must place yours to certs directory.

Edit the inventory.ini file and run ansible playbook with this command:
ansible-playbook -i inventory.ini tasks/main.yml --become-user root --become-method sudo --ask-become-pass
```
