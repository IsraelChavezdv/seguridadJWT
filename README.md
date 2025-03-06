# Seguridad JWT (Jason Web Token)

API Desarrollada con Spring Boot y MySQL

## Tecnologías utilizadas

- Java 17
- Maven 4.0.0
- MySQL 8.0
- IDE (IntelliJ)
- Spring boot 3.4.3 + Security + jsonwebtoken 0.11.5

## Configuración del Proyecto

1. **Clona el repositorio:**

   ```bash
   git clone https://github.com/IsraelChavezdv/seguridadJWT.git
   cd tu-ubicacion/proyecto

2. **Abrir el proyecto con algun IDE y ejecutar el comando mvn clean install para generar el .jar
     de la app**

3. **Puerto 8080, MYSQL puerto 3606**

4. **Correr la APP e ir Postman. Primero registrar un usuario:**
    ```bash
   (POST) http://localhost:8080/auth/signup (Registrar Usuario)
   Requiere BODY: 
   { "email":"ejemplo@ejemplo.com",
    "password":"ejemplo",
    "fullName": "Nombre Completo"
    }

5. **Con usuario registrado. Iniciar Sesión:**
    ```bash
   (POST) http://localhost:8080/auth/login (Iniciar Sesión)
   Requiere BODY: 
   { "email":"ejemplo@ejemplo.com",
    "password":"ejemplo"
    }
6. **Si es exitoso. Request successful 200 OK:**
    ```bash
    {
    "token": "copiar-cadena"
    }

 8. **Mostrar Usuario. Authorization Bearer Token: Pegar Token**
    ```bash
    (GET) http://localhost:8080/users/me (Mostrar usuario)


## Desarrollado por Israel Chávez
