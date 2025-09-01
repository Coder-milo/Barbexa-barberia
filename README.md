# ✂️ Barbexa - Barbería Online

Barbexa es una aplicación web moderna para la gestión de barberías.  
Permite a los clientes **registrarse, iniciar sesión y reservar servicios**, y a los administradores **gestionar usuarios, servicios y citas** de forma sencilla.  

El proyecto está dividido en **Frontend** (Vite + JS) y **Backend** (Node.js + Express + PostgreSQL/MySQL), con un diseño responsive y validaciones completas.

---

## 📸 Vista Previa

![Barbexa Logo](./frontend/assets/img/logo.png)

*(Agrega aquí capturas de pantalla de las vistas principales: login, register, home, etc.)*

---

## 🚀 Características

- 🔐 **Autenticación de usuarios** con login y registro seguro.  
- 🧾 **Gestión de clientes y servicios**.  
- 📅 **Reservas y control de citas**.  
- 🎨 **Frontend responsive y moderno** con Vite.  
- ⚡ **Backend con Node.js + Express**.  
- 🗄️ **Base de datos relacional** (PostgreSQL / MySQL).  
- ✅ **Validaciones avanzadas en formularios**.  
- 📂 **Arquitectura organizada** con separación de capas.

---

## 🛠️ Tecnologías

### **Frontend**
- Vite
- HTML5 + CSS3
- JavaScript (ES Modules)
- Router personalizado
- Validaciones de formularios

### **Backend**
- Node.js
- Express
- JWT (autenticación)
- Bcrypt (encriptación de contraseñas)
- PostgreSQL / MySQL

---

## 📂 Estructura del Proyecto

barbexa/
│── backend/ # Servidor Node.js + Express
│ ├── src/
│ │ ├── index.js # Punto de entrada del servidor
│ │ ├── routes/ # Rutas API (auth, users, etc.)
│ │ ├── controllers/ # Lógica de negocio
│ │ ├── models/ # Modelos DB
│ │ └── middlewares/ # Middlewares (auth, validaciones)
│ └── package.json
│
│── frontend/ # Aplicación cliente (Vite)
│ ├── index.html
│ ├── home.html
│ ├── login.html
│ ├── register.html
│ ├── style/ # Estilos CSS
│ ├── js/ # Lógica JS
│ │ ├── router.js
│ │ ├── login.js
│ │ ├── register.js
│ │ ├── home.js
│ │ └── utils.js
│ └── assets/ # Imágenes, logos, etc.
│
└── README.md

yaml
Copiar código

---

## ⚙️ Instalación y Uso

### 1️⃣ Clonar el repositorio
```bash
git clone https://github.com/Coder-milo/barbexa.git
cd barbexa
2️⃣ Configurar el Backend
bash
Copiar código
cd backend
npm install
Crear un archivo .env en backend/ con las siguientes variables:

env
Copiar código
PORT=3000
DB_HOST=localhost
DB_USER=usuario
DB_PASSWORD=contraseña
DB_NAME=barbexa_db
JWT_SECRET=supersecreto
Ejecutar el servidor:

bash
Copiar código
npm run dev
3️⃣ Configurar el Frontend
bash
Copiar código
cd frontend
npm install
npm run dev
El frontend correrá en http://localhost:5173
El backend en http://localhost:3000

🧪 Endpoints Principales
Auth
POST /api/v1/auth/register → Registro de usuario

POST /api/v1/auth/login → Inicio de sesión

Usuarios
GET /api/v1/users → Listar usuarios (admin)

GET /api/v1/users/:id → Obtener usuario por ID

Servicios
GET /api/v1/services → Listar servicios

POST /api/v1/services → Crear servicio (admin)

Reservas
GET /api/v1/bookings → Listar reservas

POST /api/v1/bookings → Crear reserva

👨‍💻 Contribución
Haz un fork del repositorio.

Crea una nueva rama: git checkout -b feature/nueva-funcionalidad.

Realiza los cambios y haz commit: git commit -m "Agregada nueva funcionalidad".

Sube tu rama: git push origin feature/nueva-funcionalidad.

Crea un Pull Request.

📜 Licencia
Este proyecto está bajo la licencia MIT.
Puedes usarlo libremente con fines educativos y de desarrollo.

💡 Créditos
Desarrollado con ❤️ por José Camilo Doria (@Coder-milo)

yaml
Copiar código

---

👉 José, este es un README **completo y profesional**.  
¿Quieres que lo deje más **formal** (tipo empresarial) o más **atractivo con emojis, badges y screenshots** estilo startup? 🚀







Preguntar a ChatGPT
