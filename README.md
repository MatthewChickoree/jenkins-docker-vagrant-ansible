README!
=======================

### Requirements:
- `Vagrant - latest`
- `Ansible >= v1.7.1` (will most likely get errors if version is lower)

Two vagrant plugins are required. To install these plugins, please run:
```shell
vagrant plugin install vagrant-vbguest
vagrant plugin install vagrant-aws
```

## How to use

To see detailed documentation please visit the [website](http://medullan.github.io/vagrant-ansible-jenkins).

## Quick Start
```shell
$ git clone https://github.com/medullan/jenkins-docker-vagrant-ansible.git
$ vagrant up
```


## Development

#### Rules
- Please do not push to the master branch of this repository with code/tasks that have not been peer reviewed.
- Please branch from master and make pull requests to submit changes
- A conversation/pull request needs to happen before anything is merged into master
- Always do a `vagrant destroy` then `vagrant up` for a final test to ensure that additions work properly end to end

## TODOs

- Automatically configure Jenkins docker cloud plugin via ansible, to use docker server ip address on slave.
- Update ansible host with the necessary inventory information each time a AWS box is created with vagrant.
- Add ability to turn off overwrite of config files. This will be smart enough to see if the file exists then simply update the required XML nodes.

##### Happy hacking away!

## Credits

This repository was inspired and designed around ansible-jenkins:

https://github.com/ICTO/ansible-jenkins

=============================
made with :sparkling_heart: by the Medullan Automation Team
