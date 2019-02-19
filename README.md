# Ansible Playground

Setup thanks to: https://rogerwelin.github.io/ansible/docker/2016/07/04/testing-ansible-playbooks-with-docker.html

This is just a simple way to play with Ansible locally.

SSH keys were generated just for this, they aren't used anywhere.

## Steps To Use

1. `$ ./build_image.sh`
2. `$ ./run_container.sh`
3. `ansible -m ping local`

You should get a success from Ansible

```
localhost | SUCCESS => {
    "changed": false,
    "ping": "pong"
}
```

At this point you can execute a playbook with `ansible-playbook playbook.yml`
