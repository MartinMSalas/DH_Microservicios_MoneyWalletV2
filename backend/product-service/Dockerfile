#Versión de Java utilizado. Tiene que estar
#instalada en el contenedor para poder ejecutar
#el proyecto
FROM openjdk:17
#Dirección del ejecutable.
#Por defecto se crea dentro de la carpeta target
ARG JAR_FILE=target/product-service.jar
#Copia el archivo y lo renombra app.jar
COPY ${JAR_FILE} app.jar
#Una vez que se encuentra dentro del contenedor
#Con entrypoint ejecuta el comando [...] para ejecutar el proyecto
ENTRYPOINT ["java","-jar","app.jar"]
#Exponemos el puerto para poder manipularlo después desde nuestra pc
EXPOSE 8081

