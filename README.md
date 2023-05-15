# DriverWN722NV2-4
####################################################################################################
#Repositorio que contiene los Drivers de la Interfaz Tp-Link WN722N V2, V3 y V4 para Kali Linux 2023.1
#Los pasos descritos a continuación se realizaron con la placa Wireless WN722N V4.0 
#sobre un Kali Linux 2023.1 Instalado el 11 de Mayo de 2023
####################################################################################################
#Pasos elaborados por @jcaitf

Antes que nada como administrador (root) de kali ejecute los siguientes comandos y realice los reboot cuando se indiquen....

1. apt update
2. apt upgrade
3. reboot


4. apt install bc build-essential libelf-dev 
5. apt-get install linux-headers-$(uname -r)
6. git clone https://github.com/jca6185/DriverWN722NV2-4.git
7. echo "blacklist r8188eu" > "/etc/modprobe.d/realtek.conf"
8. reboot


9. cd DriverWN722NV2-3
10. make
11. make install
12. reboot


ENTRAR EN MODO MONITOR:
1. iwconfig
2. airmon-ng check kill
3. airmon-ng start wlan0
4. iwconfig

NOTA:
La interfaz en modo monitor queda con el mismo nombre wlan0


