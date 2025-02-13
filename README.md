
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






