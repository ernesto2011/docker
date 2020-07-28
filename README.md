# docker

 ### Pre-requisitos 📋
 para ejecutar el programa debes tener:
 * S.O linux  
 * Python
 * docker y docker-compose

 ## Comenzando 🚀
 para usar el programa solo debes clonar el repositio o en su caso descargarlo el zip y descomprimirlo para poder usarlo
 
 Puede usar el comando:
  - git clone "link del repositorio"
   
## pruebas ⚙️
 para empezar situarse dentro de la carpeta que se creo a la hora de clonar el repositorio con el siguiente comando:
 - cd docker
 
 Compilar el contenedor (este proceso puede tardar varios minutos pues descargara varios archivos dependiendo de su internet)
- sudo docker-compose up -d

Verificar que los contenedores estén corriendo:
- sudo docker ps


## para volver a ejecutar el contenedor
para cuando vuelva a usar el proyecto debe ejecurar los comandos anteriores excepto uno:
- sudo docker-compose up -d
ahora sera

- sudo docker-compose up

asi se mantendra el servidor escuchando en todo momento y para detenerlo utlice las teclas
- ctrl+c
por si hay un error y deba reiniciarlo

## Ingresar a la dirección desde el navegador para ver la aplicación flask funcionando:
- http://localhost:8181
 esta es la pagina principal que se mostrara

- http://localhost:8181/login
 esta pagina es un login para poder ingresar pero primero debe registrarse en el formulario
 
- http://localhost:8181/signup
este es el formulario una vez registrado lo redireccionara a el login y ya logeado lo mandara a un formulario donde podra crear una publicacion

## para ver los registros en la base de datos
* primero de sebe obtener el id de servicio de mondo en otra terminal ejecutamos el comando 
  - sudo docker ps (copiamos el id de mongo)
  
 despues ejecutamos el comando
  - sudo docker exec-it "id" bash
 
 despues nos arrojara un entorno virtual de ese contenedor para probar que esta corriendo mongo en ese contenedor ejecutamos
  - mongo
  
 para ver las bases de datos ejecutamos 
  - show dbs
  
 para usar una bd usamos el comando sin comillas:
  - use "nombre de la bd"
 
 y para ver las tablas ussmos el comando sin las comillas:
  - show collections "nombre dela tabla"
 
 para ver los registor usamos el comando sin las comillas:
  - db."nombre de la tabla".find()
  
  
 ## para eliminar los registro puede usar el siguiente comando:
  - db."nombre_de_la_BD".drop()
  
  




## Construido con 🛠️

_lenguaje de programación_

* Python
* html
* framework flask
