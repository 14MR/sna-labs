# Assignment 2

The task: create docker container with ssh which is public available with ssh key, another docker container with wiki system which is accessible only through first container and not directly from internet.

How to use:
1. `docker-compose up` on the remote machine
2. create ssh tunnel to the machine `ssh -L 31337:app:3000 root@IP_ADDRESS_OF_THE_MACHINE -p 2222`
