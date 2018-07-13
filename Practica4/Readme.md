# Practica 4 de SWAP
## Pablo Navarro Guijarro

El objetivo de esta práctica es **configurar el acceso por HTTPS** a los servidores y habilitar reglas en el cortafuegos para mejorar la seguridad del servidor

Configuramos el certificado SSL autofirmado en ambos servidores

![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica4/ssl-swap1.png)
![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica4/ssl-swap2.png)
![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica4/SSLEngine-swap1.png)

Ahora configuramos el balanceador para que balancee las peticiones HTTPS tambien

![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica4/conf-nginx-https.png)

Ya hemos configurado el SSL asi que vamos a configurar el Cortafuegos. Vamos a crear un script para configurarlo y a continuación vamos a incluir el script en rc-local para que se ejecute al encender la máquina

![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica4/script-cortafuegos.png)
![imagen](https://github.com/Skeptor/SWAP1718/blob/master/Practica4/rc-local.png)
