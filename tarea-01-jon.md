# 1. Conectarse a nuestra maquina por ssh y habilitar http
Yo lo voy a hacer desde la terminal MINGW, Primero de todo me conecto a mi maquina con la clave publica del servidor
![](images/jon/captura01.png)
Lo de habilitar el http es en el apartado ***Security groups*** una vez dentro en la pestaña ***Inbound*** tenemos que añadir una regla que sea el protocolo http escuchando por el puerto 80, en mi caso ya me lo venia hecho por defecto, al crear la maquina
![](images/jon/captura03.png)

# 2. Instalacion de Apache2
Antes de instalar nada actualizaremos los repositorios
![](images/jon/captura02.png)
y ahora instalaremos el servidor apache con el siguiente comando:
![](images/jon/captura04.png)
# 3. Instalacion del servidor de Bases de datos
Una aplicacion deberá disponer de un servidor de bases de datos y al menos una base de datos a la que conectarse, podremos hacerlo instalando MYSQL con el siguiente comando
![](images/jon/captura05.png)
Y despues configurando el servidor, tras escribir otro comando
![](images/jon/captura06.png)
![](images/jon/captura07.png)
![](images/jon/captura08.png)
Tras configurarlo ya podemos logearnos en MYSQL con nuestro usuario, y empezar a trabajar con las bases de datos
![](images/jon/captura10.png)