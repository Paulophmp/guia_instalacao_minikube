# Guia Instalação Minikube
  O Minikube é uma ferramenta que facilita executar o Kubernetes localmente, executando um cluster de Kubernetes com um único nó.

## Requisitos

* kubectl
* minikube
* virtual-box
* helm

## INSTALANDO O KUBECTL
```
curl -LO https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl
```
```
sudo chmod +x kubectl && sudo mv kubectl /usr/local/bin/
```

## INSTALANDO O MINIKUBE
```
curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
```
```
sudo chmod +x minikube && sudo mv minikube /usr/local/bin/
```


## INSTALANDO VIRTUALBOX-6.0 NO UBUNTU


Para instalar o VirtualBox no Ubuntu, abra um terminal e siga os passos abaixo.

1. Importe a chave pública do repositório:

```
wget -q https://www.virtualbox.org/download/oracle_vbox_2016.asc -O- | sudo apt-key add -
```
2. Adicione o repositório do VirtualBox:
```
echo "deb [arch=amd64] http://download.virtualbox.org/virtualbox/debian bionic contrib" | sudo tee /etc/apt/sources.list.d/virtualbox.list
```
3. Atualize seus repositórios:
```
sudo apt update
```
4. Instale o VirtualBox:

```
sudo apt install virtualbox-6.0
 ```

4.1 Ou baixar .deb diretamente do site

```
[https://www.virtualbox.org/]
 ```

