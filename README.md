# ansible-kovacs
Pour le contrôle continu de Kiki


# TEST-01 :
```
cd formation-ansible/test-01/
vagrant up
```

![image](./test-01.png)

### Les pings : 

![image](./test-01-ping.png)

------------------------------------------------------
# TEST-02 :
```
cd formation-ansible/test-02/
vagrant up
```
![image](./test-02.png)


-------------------------------------------------------

# ATELIER-01 : 

## Challenge-01 :

* Démarrez la VM ubuntu depuis le répertoire atelier-01.
```
vagrant up ubuntu
```
* Connectez-vous à cette VM.
```
vagrant ssh ubuntu
```
* Rafraîchissez les informations sur les paquets.
```
sudo apt update
```
* Recherchez le paquet ansible avec les options qui vont bien.
```
apt-cache search --names-only ansible
```
* Installez le paquet officiel fourni par la distribution.
```
sudo apt install -y ansible
```
* Vérifiez si l'installation s'est bien déroulée.
```
ansible --version
```
![image](./challenge-01.png)

`version : 2.10.8`

Déconnectez-vous et supprimez la VM.
```
exit

vagrant destroy -f ubuntu
```

## Challenge-02 :

```
vagrant up ubuntu
vagrant ssh ubuntu
sudo apt update
sudo apt-add-repository ppa:ansible/ansible
apt-cache search --names-only ansible
sudo apt install -y ansible
ansible --version
```
![image](./challenge-02.png)
`version : 2.17.14`

### On remarque que la version est plus récente que la version officielle du challenge précédent.



## Challenge-03 :

```
vagrant up rocky

vagrant ssh rocky

sudo dnf install -y epel-release

sudo crb enable

sudo dnf install -y python3-pip

python3 -m venv ~/.venv/ansible

source ~/.venv/ansible/bin/activate

(ansible) $ pip install --upgrade pip

(ansible) $ pip install ansible

(ansible) $ ansible --version

(ansible) $ deactivate

exit 

vagrant destroy -f rocky
```

![image](./challenge-03.png)
`Version : 2.15.13`

-------------------------------------------------------

# ATELIER-02 : 

```


```
![image](./atelier-02.png)
