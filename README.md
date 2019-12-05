ansible-galaxy.centos.docker
================================

sudo ansible-playbook -i "localhost," --connection=local --sudo -vvvv run.yml

```
ansible-playbook -i "192.168.1.1," --ask-sudo-pass --ask-pass -u user --extra-vars "docker_compose_version=1.22.0" run.yml
```

```
ansible-playbook --ask-pass --ask-become-pass  -i "192.168.1.1," --extra-vars 'docker_compose_version=1.22.0' run.yml
```

```
ansible-playbook --ask-pass --become-method sudo --become-user root --ask-become-pass  -i "192.168.1.1," --extra-vars 'docker_compose_version=1.25.0' run.yml
```

