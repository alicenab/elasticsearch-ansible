You need to have "fullchain.pem" and "privkey.pem" obtained from letsencrypt:
```
sudo certbot certonly --manual --preffered-challenges dns
```
Edit the inventory.ini file according to your hosts and run ansible playbook with this command:
```
ansible-playbook -i inventory.ini tasks/main.yml --become-user root --become-method sudo --ask-become-pass --ask-vault-pass
```
