# 🎉 ForoHub 📚

ForoHub es una plataforma completa para gestionar cursos, foros de discusión y usuarios. 🚀

## # 🛠️ Características Principales

1. 🗂️ Gestión de cursos y perfiles.
2. 📄 Creación de tópicos y respuestas.
3. 🔐 Autenticación segura con JWT.
4. 🌐 Documentación interactiva con Swagger UI.

## # 🎯 Tecnologías Usadas

1. **Java 17** ☕
2. **Spring Boot 3** 🌱
3. **Flyway** para gestión de migraciones de base de datos 🛠️
4. **MySQL** como base de datos relacional 🗄️
5. **Swagger UI** para la documentación interactiva de la API 🖥️

## # 📥 Requisitos Previos

1. 🔧 Tener instalado **Java 17**.
2. 🐬 Instalar **MySQL** y configurar la base de datos:  


CREATE DATABASE forohub;
3.🌐 Configurar las credenciales de base de datos en application.properties:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/forohub
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña
```



# 🚀 Cómo Instalar y Ejecutar el Proyecto

### 1️⃣ Clona el repositorio:

```bash
git clone https://github.com/tu-usuario/forohub.git
```
Navega al directorio del proyecto:
bash
```cd forohub```
Compila y ejecuta el proyecto:
bash
```./mvnw spring-boot:run```
Accede a Swagger UI en:
```http://localhost:8080/swagger-ui.html 🖥️```
# 📚 Documentación de la API
🔑 Autenticación
Endpoint: /api/auth/login
Método: POST
Request Body:
json
Copy
Edit
{
  "username": "admin",
  "password": "admin123"
}
Response:
json
Copy
Edit
{
  "token": "eyJhbGciOiJIUzI1NiIsInR..."
}
👤 Usuarios
Crear Usuario:
bash
Copy
Edit
curl -X POST http://localhost:8080/api/usuarios/register \
-H "Content-Type: application/json" \
-d '{"login": "ozona.carro", "clave": "password123"}'
Obtener Usuarios: GET /api/usuarios
Actualizar Usuario: PUT /api/usuarios/{id}
Eliminar Usuario: DELETE /api/usuarios/{id}
📚 Tópicos
Crear Tópico: POST /api/topicos
Obtener Tópicos: GET /api/topicos
Actualizar Tópico: PUT /api/topicos/{id}
Eliminar Tópico: DELETE /api/topicos/{id}
💬 Respuestas
Crear Respuesta: POST /api/respuestas
Obtener Respuestas: GET /api/respuestas
Actualizar Respuesta: PUT /api/respuestas/{id}
Eliminar Respuesta: DELETE /api/respuestas/{id}
# 📊 Estructura de la Base de Datos
📐 Diagrama de Tablas
Usuarios: Gestión de usuarios y sus credenciales.
Tópicos: Organización de discusiones.
Respuestas: Almacenamiento de mensajes y soluciones.
Cursos: Catálogo de cursos disponibles.
# 🛡️ Seguridad JWT
El servicio utiliza JWT para autenticación segura.

Define api.security.secret en tu archivo application.properties:
properties
Copy
Edit
api.security.secret=tu_clave_secreta
# 🖼️ Capturas de Swagger UI
🌟 Toda la API documentada con Swagger UI.
# 🧩 Contribuciones
¡Contribuciones son bienvenidas! 🙌

Haz un fork del proyecto.
Crea una nueva rama:
bash
Copy
Edit
git checkout -b feature/nueva-funcion
Realiza tus cambios y haz un commit:
bash
Copy
Edit
git commit -m "Agrega nueva función"
Envía un pull request.
# 📞 Contacto
¿Tienes preguntas? Puedes contactarnos en:
📧 correo@forohub.com
🌐 ForoHub GitHub

🌟 ¡Gracias por usar ForoHub! 🌟

Copy
Edit

¡Listo para pegarlo directamente en tu repositorio! 🎉




