# Install Docker Engine and Docker Desktop
## Install Docker Engine
```bash
sudo apt-get update
sudo apt-get install ca-certificates curl gnupg
sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg
echo \
  "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

## Install Docker Desktop
Perform the following actions
- Go to https://docs.docker.com/desktop/install/ubuntu/#install-docker-desktop and download the **.deb package**.
- Install docker desktop
    ```bash
    sudo apt-get update
    sudo apt-get install ./docker-desktop-<version>-<arch>.deb
    ```
- Done :tada:! Happy Dockering!

## Configuring password store for linux users
Read here - https://docs.docker.com/desktop/get-started/#credentials-management-for-linux-users

## Upgrade Docker Desktop
```bash
sudo apt-get install ./docker-desktop-<version>-<arch>.deb
```
