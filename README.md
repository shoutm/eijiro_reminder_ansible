# Shoutm Ansible

## About this software
This ansible helps:
1. Installing basic packages via apt / initial setting.
2. Setting up a dev environment for EijiroReminder.
   * https://github.com/shoutm/EijiroReminder
3. Setting up a dev environment for openstack

## Prerequisites
1. You have your own ssh private key as ~/.ssh/id_rsa.
2. You have your github account.

## How to setup
1. Copy target_servers.sample to target_servers
2. Write your server IP down in target_servers

### Setting up Common dev environment
1. Type a command below.
```
$ ansible-playbook common_dev.yml -k -K -i target_servers -D
```
-k(--ask-pass) is needed only at the first time to run this script

