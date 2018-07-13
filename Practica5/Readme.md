# Practica 5 de SWAP
## Pablo Navarro Guijarro

El objetivo de esta práctica es **replicar** la base de datos del servidor principal en el servidor de backup con una estructura maestro-esclavo.

Primero creamos la tabla de la BD en ambos servidores

![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica5/create_table.png)

Tras esto configuramos el servidor principal como master en la configuración de SQL

![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica5/conf-master-sql.png)

Tras esto introducimos los datos del maestro en el servidor esclavo y comprobamos que está sincronizado
![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica5/conf-slave-sql.png)

Como podemos ver en Seconds_Behind_Master el valor está a 0 por lo que el servidor está sincronizado
