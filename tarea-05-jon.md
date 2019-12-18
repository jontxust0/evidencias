# TAREA 5: Servidor FTP
Podemos instalar el ***vsftpd*** que viene siendo el servidor FTP en GNU/Linux

![](images/tarea05md/captura01.PNG)

En el archivo de configuracion deberemos de tener escritas las siguientes lineas

![](images/tarea05md/captura03.PNG)

![](images/tarea05md/captura08.PNG)

Una vez instalado, vamos a conectarnos al servidor desde otra maquina, via comandos. para que esto sea posible, en la instancia de amazon tenemos que añadir una regla de entrada que admita conexiones por el puerto 21

![](images/tarea05md/captura04.PNG)

![](images/tarea05md/captura05.PNG)

Ahora vamos a probar a conectarnos al servidor FTP

![](images/tarea05md/captura06.PNG)

nos da respuesta, pero el usuario no es valido. Vamos a crearlos.
El usuario admin, cliente y servidor, cada uno con los directorios donde podra realizar cambios

![](images/tarea05md/captura07.PNG)

Por ultimo nos conectaremos al servidor ftp con los tres usuarios creados anteriormente, y comprobaremos que esten en su correspondiente directorio

El usuario admin

![](images/tarea05md/captura09.PNG)

El usuario cliente

![](images/tarea05md/captura10.PNG)

El usuario servidor

![](images/tarea05md/captura11.PNG)