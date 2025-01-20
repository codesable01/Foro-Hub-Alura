🎉 ForoHub 📚





ForoHub es una plataforma completa para gestionar cursos, foros de discusión y usuarios. 🚀

🛠️ Características Principales

🗂️ Gestión de cursos y perfiles.

📄 Creación de tópicos y respuestas.

🔐 Autenticación segura con JWT.

🌐 Documentación interactiva con Swagger UI.

🎯 Tecnologías Usadas

Java 17 ☕

Spring Boot 3 🌱

Flyway para gestión de migraciones de base de datos 🛠️

MySQL como base de datos relacional 🗄️

Swagger UI para la documentación interactiva de la API 🖥️

📥 Requisitos Previos

🔧 Tener instalado Java 17.

🐬 Instalar MySQL y configurar la base de datos:

CREATE DATABASE forohub;

🌐 Configurar las credenciales de base de datos en application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/forohub
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña

🚀 Cómo Instalar y Ejecutar el Proyecto

Clona el repositorio:

git clone https://github.com/tu-usuario/forohub.git

Navega al directorio del proyecto:

cd forohub

Compila y ejecuta el proyecto:

./mvnw spring-boot:run

Accede a Swagger UI en: http://localhost:8080/swagger-ui.html 🖥️

📚 Documentación de la API

🔑 Autenticación

Endpoint: /api/auth/loginMétodo: POST

Request Body:

{
  "username": "admin",
  "password": "admin123"
}

Response:

{
  "token": "eyJhbGciOiJIUzI1NiIsInR..."
}

👤 Usuarios

Crear Usuario:

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

📊 Estructura de la Base de Datos

📐 Diagrama de Tablas



🗄️ Tablas Principales

Usuarios: Gestión de usuarios y sus credenciales.

Tópicos: Organización de discusiones.

Respuestas: Almacenamiento de mensajes y soluciones.

Cursos: Catálogo de cursos disponibles.

🛡️ Seguridad JWT

El servicio utiliza JWT para autenticación segura.

📂 Configuración

Define api.security.secret en tu archivo application.properties:

api.security.secret=tu_clave_secreta

🖼️ Capturas de Swagger UI

🌟 Swagger Documentado



🛠️ Métodos Principales

Usuarios: POST, GET, PUT, DELETE

Tópicos: POST, GET, PUT, DELETE

Respuestas: POST, GET, PUT, DELETE

🧩 Contribuciones

¡Contribuciones son bienvenidas! 🙌

Haz un fork del proyecto.

Crea una nueva rama (git checkout -b feature/nueva-funcion).

Realiza tus cambios y haz un commit (git commit -m "Agrega nueva función").

Envía un pull request.

📞 Contacto

¿Tienes preguntas? Puedes contactarnos en:📧 correo@forohub.com🌐 ForoHub GitHub

🌟 ¡Gracias por usar ForoHub! 🌟
