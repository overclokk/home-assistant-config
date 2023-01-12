# home-assistant-config

🏠 Home Assistant configuration &amp; Documentation for my Smart House.

## Linux post installation

Install Docker
https://docs.docker.com/engine/install/ubuntu/
Note: do the post install to be able to run docker without sudo.

Install Docker Compose
https://docs.docker.com/compose/install/

Install git
```bash
sudo add-apt-repository ppa:git-core/ppa
sudo apt update
sudo apt install git
```

Verify git is installed:
```bash
git --version
```

## Configuration folder
First of all we need a folder to wrap Home Assistant files, in my personal case I started to create a folder in my home account called `homeassistant` and a subfolder called `config`, now you don't need a subfolder you can have a root folder if you want and I'll moe all my files ASAP to this config:

```bash
# home/my_user/
> mkdir homeassistant
```

If you create also a `config` folder and want to share also the file `compose.yml` you can have all in the same folder and use a symlink if you want for running the container from outside.


```bash
# home/my_user/homeassistant
> ls -s config/compose.yaml compose.yaml
```

