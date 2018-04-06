# Practica 2 de SWAP
## Pablo Navarro Guijarro

El objetivo de esta práctica es **sincronizar** las dos maquinas virtuales previamente configuradas para tener en ambas la misma carpeta /etc/www/

Primero probaremos a crear un tgz con los archivos de una máquina en la otra

![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica2/Prueba_copia.png)


Una vez hemos probado a hacer esto vamos a ejecutar el comando rsync para sincronizar la carpeta del segundo servidor con el servidor principal.

![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica2/rsync-manual.png)

El último paso es configurar las máquinas para que puedan conectarse por ssh sin necesidad de contraseña. Para eso generaremos un par de claves pública-privada y las almacenaremos en la otra máquina

![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica2/ssh-copy.png)

Tras esto añadimos la tarea al archivo crontab para que todas las horas el servidor se sincronice automáticamente

![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica2/crontab.png)