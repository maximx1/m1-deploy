m1-deploy
=========

### Description
Simple ansible + vagrant deployment stack

### Setup
Obtain an api key with Digital Ocean and place it in the Vagrant file along with the name you wish to store your ssh key as. If you already have an ssh key, just name it exactly as it is in DO and this will skip it.

Modify the dockerappinstaller role with your Dockerfile and app name in the main.yml.

### Command
```
~$ vagrant up
```

### Coming upgrades
external config of properties such as app naming.

### Notes
[defining hosts](https://docs.vagrantup.com/v2/provisioning/ansible.html)
