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

## 🧠 **Estructura del Proyecto**

| Archivo / Clase             | Descripción                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| `WebClientConfig.java`     | Configura el `WebClient` con la URL base de Gutendex.                      |
| `Author.java` / `Book.java`| Entidades JPA que representan autores y libros.                            |
| `AuthorRepository.java`    | Métodos para consultar autores en la base de datos.                        |
| `BookRepository.java`      | Repositorio para los libros.                                               |
| `AuthorService.java`       | Lógica para consultar y filtrar autores.                                   |
| `BookService.java`         | Lógica para importar libros, asociar autores, filtrar por idioma, etc.     |
| `BookResponse.java`        | Clase auxiliar para mapear la respuesta JSON paginada de Gutendex.         |

---

## 🛠️ **Cómo Ejecutar el Proyecto**

