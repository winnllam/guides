# Docker on Ubuntu
Steps and commands to install Docker on Ubuntu.

## Installation

### Set up to install Docker
```
sudo apt update

sudo apt install apt-transport-https ca-certificates curl software-properties-common

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"

sudo apt update

apt-cache policy docker-ce
```

### Install Docker

```
sudo apt install docker-ce

sudo systemctl status docker
```

### Run Docker without Sudo

```
sudo usermod -aG docker $USER
```
Run the above command and then restart your computer to update changes.
