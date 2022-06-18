# Provision Drupal Servers


Run playbook and use SSH server password (twice -kK)

```
ansible-playbook playbook.yml -u aberry -kK  
```

Run playbook and limit to a single server's IP address
```
 ansible-playbook playbook.yml -u aberry -kK --limit 172.16.0.14
 ```
