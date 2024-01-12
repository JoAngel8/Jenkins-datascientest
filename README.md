# Jenkins-datascientest
Jenkins DevOps - Datascientest training and practices

---

# JENKINS 

  Plugins Installed : 
  plugin github integration

# GITHUB 
Création du dépôt GitHub :
Jenkins-datascientest (Public) 

  WebHook
  - PayLoad URL activated

  - Which events would you like to trigger this webhook?
```
    Let me select individual events:

    Branch or tag creation
    Branch or tag deletion
    Packages
    Pull request review comments
    Pull requests
    Pull request reviews
    Pushes
    Registry packages
```

# Docker HUB


# VIRTUAL MACHINE

## Installations
If an installation is required  

**Kubernetes**
``` bash 
curl -sfL https://get.k3s.io | sh -s - --write-kubeconfig-mode 644
sudo kubectl version --short
k3s kubectl get nodes
```

**Helm**
``` bash
curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
chmod 700 get_helm.sh
./get_helm.sh
```

**Docker** 
``` bash
sudo apt-get install ca-certificates curl gnupg lsb-release -y
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update -y
sudo apt-get install docker-ce docker-ce-cli containerd.io -y
sudo systemctl enable --now docker
docker -v
sudo usermod -aG docker jenkins
```

**SED**
``` bash
sudo apt-get install sed -y
```

## If required applications are installed
``` bash
Kubectl installed
$ k3s kubectl get nodes

Jenkins access on Docker engine 
$ sudo usermod -aG docker jenkins

Namespaces creation
$ kubectl create namespace dev
$ kubectl create namespace staging
$ kubectl create namespace prod

```


