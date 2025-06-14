# 📚 **Alura Literatura - Spring Boot + Gutendex**

Este proyecto es una aplicación Java desarrollada con **Spring Boot** que consume la API pública de [Gutendex](https://gutendex.com) para importar libros y autores, almacenarlos en una base de datos local y realizar operaciones sobre ellos como:

- Filtrado por idioma
- Búsqueda por nombre
- Consulta de autores vivos en un año específico

---

## 🚀 **Tecnologías Utilizadas**

- **Java 17+**
- **Spring Boot**
- **Spring Data JPA**
- **Spring WebClient**
- **H2 / PostgreSQL**
- **Gutendex API**

---

## 📦 **Funcionalidades Principales**

- 🔍 Buscar libros por título o palabra clave.
- 🌐 Filtrar libros por idioma.
- 👤 Consultar autores vivos en un año determinado.
- 💾 Persistir libros y autores evitando duplicados.
- 🔄 Acceder a toda la API de Gutendex usando paginación automática.

---

## 🗃️ **Estructura del Proyecto**
![image](https://github.com/user-attachments/assets/5326d24c-ea16-4890-8dfb-b4604a8cfacb)

---

## 🗃️ **Dependencias principales**

- spring-boot-starter-data-jpa
- postgresql (driver)
- spring-boot-starter-webflux
- spring-boot-starter-test (scope test)
 -Configuración

Archivo src/main/resources/application.properties:
    spring.datasource.url=jdbc:postgresql://localhost:5432/DDBB_Books
    spring.datasource.username=${DB_USER}
    spring.datasource.password=${DB_PWD}
    spring.datasource.driver-class-name=org.postgresql.Driver
    
    spring.jpa.hibernate.ddl-auto=update
    spring.jpa.show-sql=false
    spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect

---



---

##📜 Licencia Este proyecto es de uso libre con fines educativos. Puedes modificarlo o distribuirlo con fines no comerciales. 
Se recomienda incluir mención al autor (Luis Venegas) original si se reutiliza públicamente.

