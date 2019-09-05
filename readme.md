# Samba settings using Docker

This is a set of config/script files for setting up a samba service in a Docker container.

Thanks to `stanback/alpine-samba` image.

## instruction

### install

```
$ git clone https://github.com/kennyhyun/samba.docker
$ cd samba.docker
$ ./run
$ ./adduser $USER
```
and put the password for the USER. The output will be like the following.

```
New SMB password:
Retype new SMB password:
Added user USER.
```

`./run` will start the docker container when the system boots up too.

### Map a network drive from windows

Wnd+R and put your docker machine address like `\\192.168.99.99`.

It will show Projects and Downloads. Right click one and select map network drive.

