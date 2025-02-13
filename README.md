
Pre-Requisites:

1.Update the apt package index:

```
sudo apt update
```

![image](https://github.com/user-attachments/assets/824088a8-39e8-473d-bf63-977ae3185a90)

2.Install dependencies:

```
sudo apt install \
  apt-transport-https \
  ca-certificates \
  curl \
  software-properties-common
```
![image](https://github.com/user-attachments/assets/24fb43bb-3984-4cb4-b848-9f83c1906ba0)

3. Add Docker’s official GPG key:

```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```
![image](https://github.com/user-attachments/assets/a336834e-a19b-4b96-8d14-fc0d458a0504)

4.Set up the Docker stable repository:
```
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
![image](https://github.com/user-attachments/assets/f26343b1-b5bd-4b2d-a8b9-7ff43f4749ba)

5.Update the apt package index again:

 ```
sudo apt update
```
![image](https://github.com/user-attachments/assets/7aaa3610-30ba-4caa-aa7d-3db485e2aa1b)

6. Install Docker Engine:

 ```
  sudo apt install docker-ce docker-ce-cli containerd.io
```

![image](https://github.com/user-attachments/assets/60ccc980-25ea-4d79-9649-5bab2013d6de)

7.Verify Docker installation:

```
sudo docker --version
```
![image](https://github.com/user-attachments/assets/f01dbf43-59a0-4d96-824a-579ec7faf86a)

## Install Docker Compose in GitHub Codespace:

1. Download the latest version of Docker Compose:

```
sudo curl -L "https://github.com/docker/compose/releases/download/$(curl -s https://api.github.com/repos/docker/compose/releases/latest | jq -r .tag_name)/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```
![image](https://github.com/user-attachments/assets/ff1db358-cf24-481e-a0ad-69f3f794aa0e)


2.Make Docker Compose executable:

```
sudo chmod +x /usr/local/bin/docker-compose
```
![image](https://github.com/user-attachments/assets/09c6b414-b860-4c20-b069-43cae5d0fb9b)


3. Verify Docker Compose installation:

```
docker-compose --version
```
![image](https://github.com/user-attachments/assets/48209db0-1b52-4086-bc28-99cc2ddf3761)
   














