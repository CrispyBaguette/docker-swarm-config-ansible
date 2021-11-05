# docker-swarm-config-ansible

Automating Docker Swarm configs with Ansible

The contents of this repository demonstrate the principles described [in this blog article](https://blog.bruyant.xyz/posts/automating-docker-configs/).

Running `vagrant up` will provision a debian 11 VM running a Docker Swarm, by running the `init.yaml` playbook.

Running the `rotate_config.yaml` playbook will ensure that a service is running on the Docker Swarm, and generate a new config. The contents of the new config will be accessible on port 8080 ([here](http://localhost:8080/config.html)). Details about the config are accessible through `vagrant ssh` and `docker config ls`.

# Requirements

- Ansible
- Vagrant
