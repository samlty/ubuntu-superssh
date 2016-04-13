Docker Ubuntu Supervisor with SSH
===================

1) Get clone of this repo.

> git clone git@github.com:ykocaman/ubuntu-superssh.git  
> cd ubuntu-superssh

2) copy your id_rsa.pub to ssh/know_hosts if you want.

> cat ~/.ssh/id_rsa.pub > ssh/known_hosts

3) build docker image.

> docker build --rm -t ykocaman/ubuntu-superssh:latest .

4) run image.

> docker run -d --name superssh ykocaman/ubuntu-superssh

5) connect to your sweet docker container.

> ssh user@172.17.0.2

if you didnt change password from Dockerfile line 19, default password is "user".

