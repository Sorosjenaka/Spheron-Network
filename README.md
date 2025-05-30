# Spheron-Network
Guide to install and run Spheron Network Node


Minimum Hardware Specifics
* 8 Core
* 16 GB Ram
* 100 GB SSD

  ## Install docker
  
  ```
  sudo apt update -y && sudo apt upgrade -y
  for pkg in docker.io docker-doc docker-compose podman-docker containerd runc; do sudo apt-get remove $pkg; done
  sudo apt-get update
  sudo apt-get install ca-certificates curl gnupg
  sudo install -m 0755 -d /etc/apt/keyrings
  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
  sudo chmod a+r /etc/apt/keyrings/docker.gpg

  echo \
  "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

  sudo apt update -y && sudo apt upgrade -y
  sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
  sudo chmod +x /usr/local/bin/docker-compose
  ```
  # Check Docker Version
  ```
  docker --version
  ```
  # Go to website Regist Node
  * https://fizz.spheron.network/

  # Install Spheron CLI
  ```
  curl -sL1 https://sphnctl.sh | bash
  ```
  # Generate & Start Your Fizz Node
  * You must generate command in website

  
![alt text](https://github.com/Sorosjenaka/Spheron-Network/blob/main/Screenshot%202025-05-28%20100718.png?raw=true)
  # Check Logs
  ```
  sphnctl fizz logs
  ```
  ![alt text](https://github.com/Sorosjenaka/Spheron-Network/blob/main/Screenshot%20(87).png?raw=true)
  
