#***TAREA 2: Solventar problemas de direccionamiento***
Cada vez que se apaga/inicia un servidor EC2 su IP es renovada. Por tanto cada vez que quieres conectarte por SSH debes copiar la nueva IP desde el panel de instancias EC2 en AWS. Lo deseable sería tener siempre un mismo dominio/ip para hacer tanto conexiones SSH como HTTP a nuestro servidor.

Amazon AWS permite reservar una Elastic IP.

Infórmate sobre esto, realiza los ajustes necesarios en tu cuenta de AWS para poder usar siempre la misma URL a partir de ahora, y documenta los pasos que has dado para lograrlo.

Para poner una ip elastica a una instancia de AWS, tendremos que hacerlo desde el apartado ***Elastic IP's*** y una vez dentro a ***Allocate Elastic IP adress***

![](images/tarea02md/captura01.png)

Seleccionamos la primera opcion y le damos a Allocate

![](images/tarea02md/captura02.png)

Y de momento la hemos alquilado

![](images/tarea02md/captura03.png)

Ahora tendremos que asociarla a nuestra instancia

![](images/tarea02md/captura04.png)

Escribimos el ***nombre*** y la ***ip privada*** de la instancia a la que la asociaremos, y le damos a ***Associate***

![](images/tarea02md/captura05.png)

Y ya esta, tenemos la Ip elastica creada anteriormente asociada a nuestra instancia

![](images/tarea02md/captura06.png)

Una vez asociada escribimos esa direccion IP Elastica en el navegador y nos saldra el fichero index del virtualhost del servidor apache2 que tenemos instalado en la instancia

![](images/tarea02md/captura07.png)