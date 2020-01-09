# TAREA 7: Automatizar copias de seguridad
#### CREAR LOS SCRIPT PARA CLIENTE Y SERVIDOR
Primero vamos a crear el script para el servidor,y le diremos que cada vez que este se ejecute, creara una copia de la carpeta con el proyecto, y una copia de todas las bases de datos del servidor

![](images/tarea07md/captura01.PNG)

![](images/tarea07md/captura02.PNG)

Le damos permisos. En este caso que solo el usuario root pueda ejecutarlo

![](images/tarea07md/captura03.PNG)

Ahora ejecutamos el script, y podemos ver que donde antes no habia, se han creado una backup de todas las bases de datos y una copia del proyecto de la carpeta ***www***

![](images/tarea07md/captura04.PNG)

 Vamos a repetir estos mismos pasos para crear el script para el cliente

![](images/tarea07md/captura05.PNG)

En este caso solo una copia de la carpeta del proyecto

![](images/tarea07md/captura06.PNG)

Y despues de crearlo lo ejecutamos y comprueba que funciona

![](images/tarea07md/captura07.PNG)

#### AUTOMATIZAR
Vamos a utilizar crontab para que los script creados anteriormente se vayan ejecutandose solos cada cierto tiempo.
Lo haremos editando el archivo de la ruta ***/etc/crontab***

![](images/tarea07md/captura08.PNG)

y añadiremos las siguientes lineas.
En mi caso le dire que guarde la version del proyecto para el servidor, diariamente a las 18:00. Y la copia para el cliente cada semana a las 00:00

![](images/tarea07md/captura09.PNG)

#### BORRADO AUTOMATIZADO DE BACKUPS
Al automatizar las copias de seguridad se crearán ficheros backup de forma periódica que ocuparán cada vez más espacio en disco. Teniendo en cuenta esto idea otro script para borrar los backups más antiguos de forma periódica y automatizalo con crontab.