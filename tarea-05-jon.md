# TAREA 5: Servidor FTP
Podemos instalar el ***vsftpd*** que viene siendo el servidor FTP en GNU/Linux
![](images/tarea05md/captura01.png)
En el archivo de configuracion deberemos de tener escritas las siguinetes lineas
![](images/tarea05md/captura03.png)
Una vez instalado, vamos a conectarnos al servidor desde otra maquina, via comandos. para que esto sea posible, en la instancia de amazon tenemos que añadir una regla de entrada que admita conexiones por el puerto 21
![](images/tarea05md/captura04.png)
![](images/tarea05md/captura05.png)
Ahora vamos a probar a conectarnos al servidor FTP
![](images/tarea05md/captura06.png)
nos da respuesta, pero el usuario no es valido. Vamos a crearlos.
El usuario admin, cliente y servidor, cada uno con los directorios donde podra realizar cambios
![](images/tarea05md/captura07.png)
