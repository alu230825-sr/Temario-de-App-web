# Temario-de-App-web
# Propósito de Aprendizaje 1: Comprender los fundamentos del desarrollo de aplicaciones web


<img width="1399" height="503" alt="image" src="https://github.com/user-attachments/assets/cecc12d9-52c1-46fb-b976-feb6dfd36c9c" />



## 1. Introducción al desarrollo web

### Historia y evolución del desarrollo web
El desarrollo web comenzó en la década de 1990 con la invención de la World Wide Web por Tim Berners-Lee. Inicialmente, las páginas web eran simples documentos de solo texto con enlaces (HTML). Con el tiempo, la web evolucionó para soportar imágenes, estilos (CSS), interactividad (JavaScript), y posteriormente, la llegada de tecnologías como AJAX permitió experiencias más dinámicas. Hoy en día, el desarrollo web abarca aplicaciones complejas que pueden ejecutarse tanto en navegadores como en dispositivos móviles.

### Tipos de aplicaciones web

- **Estáticas:** Son páginas cuyo contenido no cambia, a menos que el desarrollador modifique el código fuente. Se entregan tal cual están almacenadas en el servidor.
- **Dinámicas:** Generan contenido en tiempo real, generalmente utilizando bases de datos y lenguajes de servidor como PHP.
- **SPA (Single Page Application):** Aplicaciones que cargan una sola página HTML y actualizan dinámicamente el contenido conforme el usuario interactúa, sin recargar la página completa (ejemplo: Gmail).
- **PWA (Progressive Web Application):** Aplicaciones web que usan tecnologías modernas para ofrecer una experiencia similar a una app nativa, incluyendo funcionamiento offline, notificaciones push y acceso desde la pantalla de inicio.

---

## 2. Arquitectura de aplicaciones web

### Cliente-Servidor
La arquitectura cliente-servidor divide el sistema en dos partes: el cliente (navegador) que solicita información y el servidor que procesa estas solicitudes y responde. El cliente muestra la interfaz de usuario, mientras que el servidor maneja la lógica y el acceso a datos.

### Arquitectura de tres capas
- **Presentación:** Interfaz de usuario (HTML, CSS, JavaScript).
- **Lógica de negocio:** Procesamiento de datos, reglas de negocio (normalmente en el servidor, con lenguajes como PHP).
- **Datos:** Manejo y almacenamiento de información (bases de datos como MySQL).

Esta separación mejora la organización, escalabilidad y mantenimiento de la aplicación.

### REST y API-first design
- **REST (Representational State Transfer):** Es un estilo de arquitectura para diseñar servicios web que utilizan HTTP y recursos identificables por URL. Permite una comunicación sencilla y escalable entre sistemas.
- **API-first design:** Es una metodología donde el diseño de la API es el punto de partida del desarrollo, asegurando que las funcionalidades estén bien definidas y sean reutilizables por diferentes clientes (web, móvil, etc.).

---

## 3. Lenguajes y tecnologías fundamentales

- **HTML (HyperText Markup Language):** Estructura básica de las páginas web.
- **CSS (Cascading Style Sheets):** Se encarga del diseño y la presentación visual.
- **JavaScript:** Lenguaje de programación que permite la interactividad y dinamismo en la web.
- **PHP:** Lenguaje de programación del lado del servidor para crear aplicaciones web dinámicas.
- **MySQL:** Sistema de gestión de bases de datos relacional, utilizado para almacenar información de forma estructurada.

---

## 4. Control de versiones

### Git y GitHub
- **Git:** Es un sistema de control de versiones distribuido que permite registrar los cambios realizados en los archivos de un proyecto, facilitando la colaboración y el seguimiento del historial.
- **GitHub:** Plataforma basada en la nube para alojar repositorios Git, colaborar en proyectos, gestionar problemas y revisar código.

### Flujo de trabajo con ramas (branching, merge, pull requests)
- **Branching (ramificación):** Permite crear copias independientes del código para trabajar en nuevas funcionalidades sin afectar la versión principal.
- **Merge (fusión):** Combina los cambios de diferentes ramas en una sola.
- **Pull Requests:** Solicitudes para fusionar cambios de una rama a otra, permitiendo revisiones antes de integrar nuevas características al proyecto principal.

---

# Propósito de Aprendizaje 2: Desarrollar componentes y funcionalidades de una aplicación web




<img width="1460" height="730" alt="image" src="https://github.com/user-attachments/assets/7ef46de6-3d27-485f-a442-d016f6110fea" />


## 1. Diseño e implementación del frontend

### Maquetación/Wireframe/Mockup
- **Maquetación:** Es el proceso de estructurar visualmente una página web usando HTML y CSS, posicionando los elementos según el diseño deseado.
- **Wireframe:** Esquema visual básico de una interfaz, similar a un boceto, que muestra la organización y distribución de los elementos sin detalles gráficos.
- **Mockup:** Representación visual más detallada y realista del diseño final, incluyendo colores, tipografías, imágenes y estilos, pero sin funcionalidad.

### API
- **API (Interfaz de Programación de Aplicaciones):** Es un conjunto de reglas que permite que el frontend se comunique con el backend para obtener o enviar datos. Generalmente, esta comunicación se realiza a través de peticiones HTTP (GET, POST, PUT, DELETE).

---

## 2. Diseño e implementación del backend

### Servidor
- El servidor es el encargado de procesar las peticiones del cliente, ejecutar la lógica de negocio, interactuar con la base de datos y devolver una respuesta adecuada.

### Manejo de peticiones y respuestas HTTP
- El backend recibe peticiones HTTP del frontend (por ejemplo, solicitar datos o enviar formularios), las procesa y responde con datos, normalmente en formato JSON o HTML, junto con un código de estado HTTP.

### Conexión a bases de datos (MySQL, PostgreSQL, MongoDB)
- El backend se conecta a bases de datos para almacenar, consultar y modificar información.
  - **MySQL y PostgreSQL:** Bases de datos relacionales, organizan la información en tablas y relaciones.
  - **MongoDB:** Base de datos NoSQL, organiza la información en documentos tipo JSON, flexible y escalable.

---

## 3. Bases de datos

### Modelado de datos y relaciones
- Consiste en diseñar la estructura de la base de datos definiendo tablas (o colecciones), campos y las relaciones entre ellas (uno a uno, uno a muchos, muchos a muchos).

### ORM (Object Relational Mapping)
- Es una técnica que permite convertir datos entre sistemas incompatibles (como objetos en un lenguaje de programación y tablas en una base de datos relacional) automáticamente. Ejemplos de ORMs son Sequelize (Node.js), SQLAlchemy (Python) o Eloquent (Laravel/PHP).

### CRUD desde el backend
- CRUD son las operaciones básicas de una base de datos: **Crear (Create), Leer (Read), Actualizar (Update), Eliminar (Delete)**. El backend implementa estos métodos para interactuar con la base de datos a través de la API.

---

## 4. Seguridad básica en aplicaciones web

### Validación de formularios
- Es el proceso de verificar que los datos ingresados por el usuario cumplen con los requisitos necesarios (por ejemplo, formato de correo electrónico, contraseñas seguras) antes de ser procesados o almacenados.

### Autenticación y autorización
- **Autenticación:** Es el proceso de verificar la identidad de un usuario, normalmente a través de un login (usuario y contraseña).
- **Autorización:** Es el proceso de asignar permisos y controlar qué recursos o acciones puede realizar un usuario autenticado, asegurando que solo accedan a lo que tienen permitido.

---

# Propósito de Aprendizaje 3: Implementar y desplegar una aplicación web funcional



<img width="1946" height="1134" alt="image" src="https://github.com/user-attachments/assets/d1bf23a0-9e13-4ca6-8962-90a11958dc64" />


## 1. Integración de frontend y backend

### Interfaz de usuario Frontend
El **frontend** es la parte visible de la aplicación con la que interactúa el usuario. Incluye todos los elementos gráficos, formularios, botones y la navegación de la web. El desarrollo frontend utiliza tecnologías como HTML, CSS y JavaScript, y frameworks/librerías como React, Vue o Angular para crear experiencias interactivas y responsivas.

### Manejo de API
La **API** (Interfaz de Programación de Aplicaciones) permite la comunicación entre el frontend y el backend. El frontend envía solicitudes a la API (por ejemplo, para obtener datos de usuarios o enviar formularios) mediante protocolos como HTTP, generalmente usando métodos como GET, POST, PUT y DELETE. El backend procesa estas solicitudes y responde con los datos necesarios, normalmente en formato JSON.

### Proceso de Solicitud y Respuesta de Backend
Cuando el usuario interactúa con la aplicación (por ejemplo, enviando un formulario), el frontend envía una **solicitud HTTP** al backend. El backend recibe esta solicitud, ejecuta la lógica requerida (validaciones, consultas a la base de datos, etc.), y envía una **respuesta** al frontend, que puede incluir datos, mensajes de éxito o error. Este ciclo permite la integración fluida entre las dos partes de la aplicación.

---

## 2. Almacenamiento en Servidor

### Tipos de servidores
- **Servidor físico:** Computadora dedicada exclusivamente a alojar y ejecutar aplicaciones web.
- **Servidor virtual (VPS):** Espacio virtualizado dentro de un servidor físico, que funciona como un servidor independiente.
- **Servidor en la nube:** Infraestructura proporcionada por plataformas como AWS, Azure o Google Cloud, con escalabilidad y administración flexible.

### Servidores y servicios de hosting
- **Hosting compartido:** Varios sitios web comparten los recursos de un mismo servidor, es económico pero con recursos limitados.
- **Hosting dedicado:** Un servidor exclusivo para un solo sitio o aplicación, con mayor control y rendimiento.
- **Hosting en la nube:** Recursos distribuidos en varios servidores, permitiendo escalar la aplicación según la demanda.

### Proveedores de Servicios de Almacenamiento
- **Amazon Web Services (AWS):** Ofrece servicios como EC2 (servidores virtuales) y S3 (almacenamiento de archivos).
- **Microsoft Azure:** Plataforma de computación en la nube con servicios de hosting y bases de datos.
- **Google Cloud Platform:** Soluciones escalables para despliegue y almacenamiento.
- **Otros proveedores populares:** DigitalOcean, Heroku, Vercel, Netlify.

---

## 3. Optimización y rendimiento

### Optimización de recursos (imágenes, scripts)
- **Imágenes:** Comprimir imágenes, usar formatos modernos (WebP), y cargar solo las necesarias (lazy loading) para mejorar la velocidad.
- **Scripts:** Minimizar, comprimir y combinar archivos JavaScript y CSS para reducir el tiempo de carga. Usar técnicas como carga asíncrona y deferida.

### Despliegue de aplicaciones web
- **Despliegue:** Proceso de publicar la aplicación en un servidor o servicio de hosting para que esté accesible a los usuarios.
- **Herramientas comunes:** FTP/SFTP, Git, plataformas como Vercel, Netlify, Heroku, o mediante pipelines automatizados.

### CI/CD básico
- **CI/CD (Integración Continua/Entrega Continua):** Prácticas que automatizan la integración de cambios de código, ejecución de pruebas y despliegue a producción. Herramientas como GitHub Actions, GitLab CI o Jenkins permiten crear flujos automatizados para asegurar calidad y rapidez en el desarrollo.

### Documentación del proyecto
- La **documentación** explica cómo instalar, configurar, y utilizar la aplicación. Incluye instrucciones para desarrolladores y usuarios finales, detalles de la arquitectura, endpoints de la API, y cualquier otra información relevante para el correcto uso y mantenimiento del proyecto.

