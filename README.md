# Setup 

# General Information 

This is my personal pi Setup 

I'm currently using a raspberry Pi 3 Model B. The pis only job is to monitor my homeserver and the VMS, Containers, Services etc. using uptime Kuma inside docker. 

# Ansible 

The Ansible Playbook will create a User and a group called admind. That's kind of my standard user name on debian servers for non root users. 

It will also install cli tools that use on all my debian servers as well. Midnight Commander, htop etc. 

Additionaly it will install docker and docker-compose. 

SSH will also be setup by copying a public key and editing the sshconfigd file. 

# Backup 

I'll propably use restic with sftp to backup the perstistant data of the docker Container