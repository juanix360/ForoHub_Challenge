# ForoHub System

ForoHub es una solución innovadora desarrollada con Spring Boot que facilita la creación y administración de foros educativos. Su diseño robusto asegura una experiencia confiable y eficiente para gestionar usuarios, temas, cursos y respuestas.

---

## **Introducción**
ForoHub tiene como objetivo proporcionar una plataforma flexible y segura para el intercambio de ideas y conocimientos a través de foros temáticos. Es ideal para entornos educativos que buscan conectar a estudiantes, profesores y administradores de cursos.

---

## **Características Principales**
- **Gestión de Usuarios**: Sistema de autenticación y autorización basado en JWT para mayor seguridad.
- **Foros Dinámicos**: Permite la creación, visualización y gestión de temas y respuestas.
- **Integración con Cursos**: Relaciona temas y foros con cursos específicos para una experiencia organizada.
- **Documentación Clara**: API documentada mediante Swagger para facilitar la integración y el uso.
- **Seguridad Avanzada**: Implementación de roles y permisos con Spring Security para controlar accesos.

---

## **Estructura del Sistema**
El sistema sigue una arquitectura modular por capas para garantizar su mantenibilidad y escalabilidad:
- **Capa API**: Contiene los controladores REST y las configuraciones relacionadas con la seguridad.
- **Capa de Negocio**: Administra las entidades principales, los repositorios y los DTOs.
- **Capa de Infraestructura**: Configura la conexión con la base de datos, gestiona errores y proporciona documentación.

---

## **Herramientas y Tecnologías**
- **Lenguaje de Programación**: Java 17
- **Framework**: Spring Boot
- **Seguridad**: Spring Security con autenticación JWT
- **Gestión de Datos**: Spring Data JPA y Hibernate
- **Base de Datos**: MySQL
- **Documentación API**: SpringDoc OpenAPI (Swagger)

---

## **Guía de Instalación**

### **Requisitos Previos**
- Tener instalado JDK 17 o superior
- Maven 3.8 o superior
- MySQL 8.0 o una versión compatible

### **Pasos para la Instalación**
1. Clona el repositorio desde GitHub:

```bash
git clone https://github.com/castleortiz1/Challenge-ForoHub-AluraLatam
cd forohub
```

2. Configura la base de datos:
   - Crea una base de datos llamada `forohub` en MySQL.
   - Actualiza el archivo `application.properties` con tus credenciales:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/forohub
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña
```

3. Construye y ejecuta la aplicación:

```bash
mvn clean install
mvn spring-boot:run
```

4. Accede a la documentación interactiva de la API en:
[http://localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)

---

## **Principales Endpoints**

| Método | Endpoint                  | Funcionalidad                          |
|--------|---------------------------|----------------------------------------|
| POST   | /auth/login               | Inicia sesión y genera un token JWT.   |
| GET    | /users                    | Recupera la lista de usuarios.         |
| GET    | /topics                   | Muestra todos los temas disponibles.   |
| POST   | /topics                   | Crea un nuevo tema en el foro.         |
| GET    | /courses                  | Lista todos los cursos registrados.    |
| POST   | /responses                | Publica una respuesta en un tema.      |

---

## **Cómo Contribuir**
¡Nos encantaría contar con tu ayuda para mejorar ForoHub! Sigue estos pasos para contribuir:
1. Realiza un fork del repositorio.
2. Crea una rama para tu nueva funcionalidad o corrección:

```bash
git checkout -b feature/nueva-funcionalidad
```

3. Realiza tus cambios y registra el commit:

```bash
git commit -m "Descripción de los cambios realizados"
```

4. Sube tu rama al repositorio remoto:

```bash
git push origin feature/nueva-funcionalidad
```

5. Envía un pull request detallando tus modificaciones.

---

## **Licencia**
ForoHub está disponible bajo la Licencia MIT. Revisa el archivo `LICENSE` incluido en este repositorio para obtener más detalles.

---

¡Gracias por elegir ForoHub! Si tienes dudas o sugerencias, abre un issue en el repositorio o ponte en contacto con nosotros.
