# docker-ubuntu-ansible
Ubuntu docker container with built-in Ansible for playbook and role testing

# The main goal
Keep all version in one repository under different tags

## Tags
- `18.04`. Ubuntu 18.04 LTS (Bionic Beaver)
- `20.04`. Ubuntu 20.04 LTS (Focal Fossa)
- `22.04`. Ubuntu 22.04.2 LTS (Jammy Jellyfish)
- `24.04`. Ubuntu 22.04.2 LTS (Noble Numbat)

## How to Build

To build the image on your own locally, do the following:

  1. [Install Docker](https://docs.docker.com/engine/installation/).
  2. `cd` into target directory. For example, target directory for `Ubuntu 24.04` is `ubuntu24.04`
  3. Run `docker build -t docker-ubuntu-ansible .`.

  ## How to Use

  1. [Install Docker](https://docs.docker.com/engine/installation/).
  2. Pull pre-build image via `docker image pull kirillzak/docker-ubuntu-ansible:latest` or build image.
  3. Run a container from the image: `docker run --detach --privileged --volume /sys/fs/cgroup:/sys/fs/cgroup:ro docker-ubuntu-ansible:latest`

## Author

[Kirill Ziuzin](https://kirill-zak.ru/)

### Thanks
Thanks for [Jeff Geerling](https://github.com/geerlingguy)

### Based
Based on:
- https://github.com/geerlingguy/docker-ubuntu1804-ansible
- https://github.com/geerlingguy/docker-ubuntu2004-ansible
- https://github.com/geerlingguy/docker-ubuntu2204-ansible
