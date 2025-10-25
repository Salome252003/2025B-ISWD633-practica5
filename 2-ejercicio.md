# Ejercicio
Configurar SonarQube utilizando Docker Compose, para esto necesitas dos servicios:
- Servicio: SonarQube
- Desde el host es necesario acceder a SonarQube por lo que necesitas mapear el puerto correspondiente.
- Servicio: PostgreSQL (existen otras opciones: Microsoft SQL Server, Oracle)
- Coloca un healtcheck para cada uno de los servicios.
- Los dos servicios deben pertenecer a una red de tipo bridge
- Investiga cuáles son los volúmenes necesarios para cada servicio
- Investiga cuáles son las variables de entorno para que los servicios funcionen de manera adecuada.
  
# Una vez creado tu archivo .yaml realiza la respectiva prueba 
# COMPLETAR CON UNA CAPTURA DE PANTALLA LUEGO DE EJECUTAR EL ARCHIVO
# ACCEDER A LOCALHOST:puertoDefinido para ingresar a SonarQube

1. Primero creamos la carpeto donde guardaremos nuestro .yaml

<img width="806" height="305" alt="image" src="https://github.com/user-attachments/assets/e3cd1fa1-18da-413d-a76a-5e1f4f1014c7" />

2. Segundo colocamos el correspondiente texto en el .yaml

<img width="1380" height="715" alt="image" src="https://github.com/user-attachments/assets/712e866e-167e-4ac4-a72c-98b09daa7890" />

3. Luego levantamos solo la base de datos con el siguinte comando

docker compose up -d postgres

<img width="1447" height="465" alt="image" src="https://github.com/user-attachments/assets/7a099372-889c-4ef0-bb1c-ce91f2fb5dbd" />

4. Verificar que PostgreSQL está corriendo con el siguiente comando

docker compose ps

<img width="1457" height="167" alt="image" src="https://github.com/user-attachments/assets/66e25851-5ec6-4eeb-86db-a6e0f2e04443" />

5. En el archivo .yaml completamos con todo lo que falte (volumenes)

<img width="1748" height="902" alt="image" src="https://github.com/user-attachments/assets/0fd75521-7781-4020-bf28-0631613c8244" />

6. Volvemos a correr los comandos de los pasos anteriores

<img width="1453" height="137" alt="image" src="https://github.com/user-attachments/assets/3efa267f-c315-4102-9cfc-d9c645c3ed5b" />

7. Por ultimo entramos a la página: http://localhost:9000

<img width="1918" height="1021" alt="image" src="https://github.com/user-attachments/assets/26f3a557-598f-4162-a1f5-90afa2319760" />

<img width="1917" height="950" alt="image" src="https://github.com/user-attachments/assets/9ec765da-cb6a-42fb-8a26-e1633e8d3f9f" />



