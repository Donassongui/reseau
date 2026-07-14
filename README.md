# Doccumentation de mon architecture reseau
1- schéma reseau



<img width="613" height="258" alt="image" src="https://github.com/user-attachments/assets/9a0fbd86-4005-4e88-a1e8-2a582aaf2924" />








2-Adresses utilisées
```Bash
Adresse réseau: 192.168.100.0/24
VM-1: 192.168.100.1/24
VM-2: 192.168.100.2/24
```

3-Commande utilisées
```Bash
##Pour la configuration réseau##
#VM-1:# 
sudo ip addr add 192.168.100.1/24 dev eth0
sudo ip link set eth0 up (Pour avtivé l'interface eth0)
ip a (Pour vérifier que l'adresse a été atribuer au l'interface eth0)
#VM-2#
sudo ip addr add 192.168.100.2/24 dev eth0
sudo ip link set eth0 up (Pour avtivé l'interface eth0)
ip a (Pour vérifier que l'adresse a été atribuer au l'interface eth0)
##Test de connectivité##
#VM-1#
#Avec ping
Ping 192.168.100.2
#Avec traceroute
trace route 192.168.100.2
#VM-2#
#Avec ping
ping 192.168.100.1
#Avec trace route
traceroute 192.168.100.1
```
