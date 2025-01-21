

# **Foro Hub API**

**Foro Hub** es una API RESTful para gestionar un foro donde los usuarios pueden crear, leer, actualizar y eliminar (CRUD) tópicos. La API está construida con **Spring Boot** y **MySQL** para el almacenamiento de datos. El sistema permite la autenticación básica para acceder a ciertas rutas, específicamente las que gestionan los tópicos del foro.


## **Tecnologías**

- **Spring Boot**: Framework para la creación de la API RESTful.
- **JPA (Java Persistence API)**: Para la gestión de la base de datos.
- **MySQL**: Sistema de gestión de bases de datos para almacenar los tópicos.
- **JWT**: Para la generación y validación de tokens (si se implementa una autenticación más avanzada en el futuro).

## **Endpoints principales**

### **Base URL**: `/api`
### **Tópicos**

- **GET** `/topicos`: Obtener todos los tópicos (requiere autenticación).
- **POST** `/topicos`: Crear un nuevo tópico (requiere autenticación).
- **PUT** `/topicos/{id}`: Actualizar un tópico existente (requiere autenticación).
- **DELETE** `/topicos/{id}`: Eliminar un tópico (requiere autenticación).

### **Autenticación de usuarios**

- **POST** `/auth/register`: Registro de un nuevo usuario (sin autenticación).
- **POST** `/auth/login`: Inicio de sesión y generación de JWT (sin autenticación).

