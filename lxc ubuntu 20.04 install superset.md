


IP：192.168.1.166/24
#### Install using the repository
1. Set up the repository
```
$ sudo apt-get update
$ sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
	
```
2. Add Docker’s official GPG key:
```
 curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```

```
sudo echo \
  "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

```
install docker engine

```
 sudo apt-get update
 $ sudo apt-get install docker-ce docker-ce-cli containerd.io
```
###### Proxmox VE 下的 LXC 內跑 Docker-CE
巢狀支援
https://www.pigo.idv.tw/archives/3322
![](Pasted%20image%2020210801200136.png)
![](Pasted%20image%2020210801200016.png)

why fail at first time?
1. LXC巢狀支援
2. 硬碟及記憶體