# docker

 ## Comenzando 🚀
 para usar el programa solo debes clonar el repositio o en su caso descargarlo el zip y descomprimirlo para poder usarlo
 
 ### Pre-requisitos 📋
 para ejecutar el programa debes tener:
 * S.O linux  
 * Python
 
      
## pruebas ⚙️
 Compilar el contenedor (este proceso puede tardar varios minutos)
- cd basic_flaskapp_container
- sudo docker-compose up -d

para ver los registros en la base de datos
* primero de sebe obtener el id de servicio en otra terminal ejecutamos el comando 
  - sudo docker ps (copiamos el id de mongo)
 despues ejecutamos el comando
  - sudo docker exec-it <id> bash
 despues nos arrojara un entorno virtual de ese contenedor para probar que esta corriendo mongo en ese contenedor ejecutamos
  - mongo
 para ver las bases de datos ejecutamos 
  - show dbs
 para usar una bd usamos el comando
  - use <nombre de la bd>
 y para ver las tablas ussmos el comando
  - show collections <nombre dela tabla>
 para ver los registor usamos el comando
  - db.<nombre de la tabla>.find()

Verificar que los contenedores estén corriendo:
- sudo docker ps

Ingresar a la dirección desde el navegador para ver la aplicación flask funcionando:
- http://localhost:8181
## Construido con 🛠️

_lenguaje de programación_

* Python
* html
* framework flask
