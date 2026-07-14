# Doccumentation de mon architecture reseau
1- schéma reseau
![Screenshot](images/screenshot.png)
<img width="575" height="254" alt="image" src="https://github.com/user-attachments/assets/06b2af57-e363-44f2-a80b-2bd3f4654a8e" />










2-Adresses utilisées
Adresse réseau: 192.168.100.0/24
VM-1: 192.168.100.1/24
VM-2: 192.168.100.2/24

3-Commande utilisées
**Pour la configuration réseau**
*VM-1:* 
sudo ip addr add 192.168.100.1/24 dev eth0
sudo ip link set eth0 up (Pour avtivé l'interface eth0)
ip a (Pour vérifier que l'adresse a été atribuer au l'interface eth0)
*VM-2*
sudo ip addr add 192.168.100.2/24 dev eth0
sudo ip link set eth0 up (Pour avtivé l'interface eth0)
ip a (Pour vérifier que l'adresse a été atribuer au l'interface eth0)
**Test de connectivité**
*VM-1*
*Avec ping
Ping 192.168.100.2
*avec traceroute
trace route 192.168.100.2
*VM-2*
*Avec ping
ping 192.168.100.1
*Avec trace route
traceroute 192.168.100.1
