# Provision Drupal Servers


Run playbook and use SSH server password (twice -kK)

```

ansible-playbook playbook.yml -u aberry -kK  

```

```
  -K, --ask-become-pass  ask for privilege escalation password
  -k, --ask-pass         ask for connection password
```

>  Ansible uses SSH keys by default. --ask-pass will prompt for your SSH password instead. 
> --ask-become-pass will prompt for your password to become root (by default) when used along with --become.

Run playbook and limit to a single server's IP address
```

 ansible-playbook playbook.yml -u aberry -kK --limit 172.16.0.14

```

INstalled libraries


```
ansible-galaxy collection install community.general
```
- control Apache modules with `community.general.apache2_module`
