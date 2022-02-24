# Minha instalação Docker e Docker Composer


Instalar **Docker:**

```shell
sudo apt-get update
sudo apt install docker.io
docker --version
```

Instalação do **curl**

```shell
sudo apt install curl
curl --version
```

Instalar e configurar o **Docker Compose**

* Documentação **Docker Compose:**

>Link para Download: https://docs.docker.com/compose/install
 
* Instalar pacotes de dependência:
```shell
sudo apt-get install python3-pip python3-dev python3-dev libffi-dev libssl-dev gcc libc6-dev rustc make

```
**Docker Compose:**
```shell
sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
docker-compose --version
```

Removendo sudo do **Docker**

```shell
sudo usermod -aG docker $USER
```
* Necessário reiniciar:
```shell
su - $USER
```
