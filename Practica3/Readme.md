# Practica 3 de SWAP
## Pablo Navarro Guijarro

El objetivo de esta práctica es **configurar un balanceador de carga** para gestionar las llamadas a las maquinas virtuales

Primero configuraremos la máquina con nginx

Ésta es la configuración que tendrá nginx para gestionar las entradas

![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica3/conf-nginx.png)

Éste es el resultado de hacer peticiones al balanceador de carga

![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica2/balanceo-nginx.png)


Después de ésto configuramos la máquina dos con Haproxy. Ésta es la configuración y el resultado

![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica2/conf-haproxy.png)

![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica2/balanceo-haproxy.png)
