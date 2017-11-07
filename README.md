# simple-ansible
A docker container with ansible installed. Designed to mount an ansible project and run ansible playbooks.

`ENTRYPOINT` is ansible-playbook \
`WORKDIR` is /var/ansible_proj_root \
[Dockerfile](https://github.com/gmorse81/docker-ansible-playbook/blob/master/Dockerfile)
 

Usage: \
Something like this: \
`docker run -it -v ${PWD}:/var/ansible_proj_root gmorse81/simple-ansible:latest myplaybook.yml`