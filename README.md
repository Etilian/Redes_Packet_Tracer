## Trabajo de redes ##
- Crear cinco redes:  

1- Crear tres subredes (VLSM), una que soporte 100 host, otra que soporte 30 y por último una para 6 host. Sólo esta última podrá salir fuera. Cada una tendrá cuatro ordenadores conectados.

Para esto hemos hecho el calculo de las mascaras y nos dio que las ip utilizables son: 
	
La primera va desde la red 192.168.0.1 hasta la 192.168.0.126 y su mascara es 255.255.255.128

La segunda va desde la red 192.168.0.129 hasta la 192.168.0.158 y su mascara es 255.255.255.224

La tercera va desde la 192.168.0.161 hasta la 192.168.0.166 y su mascara es 255.255.255.240 En esta ultima se pone la puerta de enlace 192.168.0.166 que es la dirección ip del fast donde hemos conectado el router.

2- 8 ordenadores con DHCP.

Para esto hemos conectado 8 pc en un switch y este con servidor. En el servidor hemos configurado el DHCP para que de IP dinámicas desde la 1 a la 255 también hemos configurado la puerta de enlace para que los PCs tenga salido fuera.

3- 4 ordenadores con DHCP.

En este caso hemos hecho lo mismo pero con 4 PCs solo.

4- 4 ordenadores con IP fija, un punto de acceso con 5 ordenadores con DHCP.

Para esto hemos puesto 5 PCs con una ip fija que va desde la 192.168.3.2 hasta la 192.168.3.6 conectados a switch hemos conectado a este un punto de acceso y un servidor con DHCP que hemos configurado para que de ip dinámica a los 4 PCs restantes.

5- 5 ordenadores con IP fija.

Hemos conectado 5 PCs con una ip fija que va desde la 192.168.4.2 hasta 192.168.4.6

- Todas las redes estarán conectadas mediante routers.  


Para esto hemos puesto 5 routers modelo 1841 los cuales hemos conectado por el fast 0/0 a los switch de cada red. Hemos configurado los servidores y PCs de cada red para que la ip del fast de cada router sea la puerta de enlace de cada red.

Después hemos enrutado todos los routers con las ip de los seriales por los que están conectados.

- Tendremos tres servidores web:  


1- www.albacete.es : muestra una foto de Albacete.

2- www.wagner.de : muestra una foto de Wagner.

3- www.dilar.com : muestra una toto de Dílar.

Para esto hemos guardado en tres servidores cada una de las paginas y las hemos asociado con la ip de cada servidor. Hemos utilizados un cuarto servidor para que las demás redes puedan visitar las paginas con total normalidad. Dándole a cada puesto la ip de este servidor en el DNS.

- Todas las redes deben estar etiquetadas.  


Por ultimo hemos etiquetado todas las ip fijas los fast y los seriales.
