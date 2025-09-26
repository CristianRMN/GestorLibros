# Gestor de Libros 📚

Proyecto desarrollado en **Java** con **Spring Boot**, consistente en una **aplicación backend** para la gestión de libros mediante una arquitectura de **microservicios**.  
El objetivo del proyecto fue aplicar conceptos de **arquitectura distribuida**, **comunicación entre microservicios** y **persistencia en bases de datos relacionales y no relacionales**.

---

## 🚀 Arquitectura y Microservicios
El proyecto está compuesto por **4 microservicios** principales:

1. **con-external**  
   - Se encarga de la **entrada de datos** (registro y consultas de libros).  

2. **prd-rex**  
   - Gestiona el **envío de libros** a los microservicios de consulta (`relational-query` y `non-relational-query`).  
   - Al registrar un libro, también guarda los datos en **ficheros XML**.  

3. **relational-query**  
   - Microservicio encargado de la **gestión y consulta de libros** en una **base de datos relacional PostgreSQL**.  

4. **non-relational-query**  
   - Microservicio encargado de la **gestión y consulta de libros** en una **base de datos no relacional MongoDB**.  

Los microservicios se comunican entre sí usando **Feign Client**, garantizando modularidad y separación de responsabilidades.

---

## 🛠️ Tecnologías utilizadas
- **Java 17**  
- **Spring Boot**  
- **JPA/Hibernate** (para persistencia en bases de datos relacionales)  
- **Maven** (gestión de dependencias y construcción de proyectos)  
- **API REST** (exposición de endpoints para cada microservicio)  
- **Feign Client** (comunicación entre microservicios)  
- **JSON** (formato de intercambio de datos)  
- **XML** (almacenamiento de libros en ficheros)  
- **PostgreSQL y MongoDB** (persistencia relacional y no relacional)  

---

## 📚 Lo que aprendí con este proyecto
- Diseño y desarrollo de **arquitectura basada en microservicios**.  
- Comunicación entre servicios mediante **Feign Client y REST APIs**.  
- Persistencia de datos en **bases relacionales y no relacionales**, entendiendo sus diferencias y usos.  
- Manejo de **JPA/Hibernate** para consultas complejas y mapeo de entidades.  
- Creación de **ficheros XML** para almacenamiento alternativo de información.  
- Organización de un proyecto modular y escalable usando **Spring Boot y Maven**.  

---

## 💡 Próximas mejoras (ideas futuras)
- Implementar **autenticación y autorización** con Spring Security.  
- Añadir **bus de eventos o mensajería** (Kafka o RabbitMQ) para mejorar comunicación asíncrona entre microservicios.  
- Crear **documentación Swagger/OpenAPI** para todos los microservicios.  
- Añadir **tests unitarios e integración** para garantizar la robustez del sistema.  

---

## 👤 Autor
- **Cristian Regueiro Martínez**  
[LinkedIn](https://www.linkedin.com/in/cristian-regueiro-mart%C3%ADnez-084187251) | [GitHub](https://github.com/CristianRMN)
