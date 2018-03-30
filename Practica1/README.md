#Practica 1 de SWAP
##Pablo Navarro Guijarro

El primer objetivo de esta práctica era **crear** dos maquinas virtuales configuradas con Ubuntu Server y LAMP.
El segundo objetivo era **configurar** las máquinas para que pudieran "comunicarse" (*curl*) entre si.

Primero instalamos Ubuntu Server y configuramos una direccion IP estática de la máquina, editando el archivo /etc/netwok/interfaces, para asegurarnos de que no cambie a causa de la red.
El resultado es que nuestras máquinas tienen las siguientes IP:

![img](https://github.com/Skeptor/SWAP1718/blob/master/Practica1/ip-maquina1.png)
![img](https://github.com/Skeptor/SWAP1718/blob/master/Practica1/ip-maquina2.png)


Una vez nuestras máquinas están configuradas y tienen los valores de red asignadas añadimos en /var/www/html un fichero llamado **hola.html** donde indicaremos simplemente en que maquina (1 o 2) nos encontramos.
Una vez lo hemos añadido desde la otra máquina ejecutamos el comando curl para obtener el fichero hola.html de la primera máquina, y así asegurar que ambas máquinas pueden interactuar.

![img](https://github.com/Skeptor/SWAP1718/blob/master/Practica1/Curl-maquina1.png)
![img](https://github.com/Skeptor/SWAP1718/blob/master/Practica1/Curl-maquina2.png) 

El último paso es conectarnos via SSH desde una máquina a la otra, y viceversa. Adjunto las capturas de pantalla de ambas conexiones. En la segunda maquina no aparece la opción de aceptar la huella digital porque está aceptada en una conexión anterior de prueba.

![img](https://github.com/Skeptor/SWAP1718/blob/master/Practica1/ssh-maquina1.png)
![img](https://github.com/Skeptor/SWAP1718/blob/master/Practica1/ssh-maquina2.png)