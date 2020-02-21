# Guia nstalacao Minikube
[ Descomplicando o Kubernetes ] - KUBERNETES e INSTALANDO o MINIKUBE

## INSTALANDO O KUBECTL
```
# curl -LO https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl
```
```
# sudo chmod +x kubectl && sudo mv kubectl /usr/local/bin/
```

INSTALANDO O MINIKUBE -- latest
```
# curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
```
```
# sudo chmod +x minikube && sudo mv minikube /usr/local/bin/
```


INSTALANDO VIRTUALBOX-6.0 NO UBUNTU 18.04 LTS


Para instalar o VirtualBox-6.0 no Ubuntu 18.04 LTS e também no Linux Mint 19, abra um terminal e siga os passos abaixo.

1. Importe a chave pública do repositório:

 wget -q https://www.virtualbox.org/download/oracle_vbox_2016.asc -O- | sudo apt-key add -

2. Adicione o repositório do VirtualBox:

 echo "deb [arch=amd64] http://download.virtualbox.org/virtualbox/debian bionic contrib" | sudo tee /etc/apt/sources.list.d/virtualbox.list

3. Atualize seus repositórios:

 sudo apt update

4. Instale o VirtualBox:

 sudo apt install virtualbox-6.0
 

sudo minikube start --vm-driver=none
