# ✂️ Barbexa - Barbería Online

**Barbexa** es una aplicación web moderna para la gestión de barberías.  
Permite a los clientes **registrarse, iniciar sesión y reservar servicios**, y a los administradores **gestionar usuarios, servicios y citas** de forma sencilla.  

El proyecto está dividido en **Frontend** (Vite + JavaScript) y **Backend** (Node.js + Express + PostgreSQL/MySQL), con un diseño **responsive**, validaciones completas y autenticación segura.

---

## 🚀 Características

- 🔐 **Autenticación de usuarios** con login y registro seguro (JWT + Bcrypt).  
- 👤 **Gestión de clientes y administradores**.  
- 💈 **Control de servicios y precios**.  
- 📅 **Reservas y control de citas** en tiempo real.  
- 🎨 **Frontend responsive y moderno** (Vite + CSS3).  
- ⚡ **Backend escalable** con Express.  
- 🗄️ **Base de datos relacional** (PostgreSQL / MySQL).  
- ✅ **Validaciones avanzadas en formularios** en frontend y backend.  
- 📂 **Arquitectura organizada** con separación de capas.  
- 🌐 **Diseño accesible y SEO-friendly**.  

---

## 🛠️ Tecnologías

### **Frontend**
- [Vite](https://vitejs.dev/)  
- HTML5 + CSS3  
- JavaScript (ES Modules)  
- Router personalizado  
- Validaciones de formularios  

### **Backend**
- [Node.js](https://nodejs.org/)  
- [Express](https://expressjs.com/)  
- JWT (autenticación)  
- Bcrypt (encriptación de contraseñas)  
- PostgreSQL / MySQL  
- Dotenv para variables de entorno  

---

## 📂 Estructura del Proyecto

```bash
barbexa/
│── backend/                # Servidor Node.js + Express
│   ├── src/
│   │   ├── index.js        # Punto de entrada del servidor
│   │   ├── routes/         # Definición de rutas API (auth, users, services, bookings)
│   │   ├── controllers/    # Lógica de negocio
│   │   ├── models/         # Modelos de base de datos
│   │   └── middlewares/    # Middlewares (auth, validaciones)
│   └── package.json
│
│── frontend/               # Aplicación cliente (Vite)
│   ├── index.html
│   ├── home.html
│   ├── login.html
│   ├── register.html
│   ├── assets/             # Imágenes, logos, íconos
│   ├── style/              # Estilos CSS
│   └── js/                 # Lógica JS
│       ├── router.js
│       ├── login.js
│       ├── register.js
│       ├── home.js
│       └── utils.js
│
└── README.md
⚙️ Instalación y Uso
1️⃣ Clonar el repositorio
bash
Copiar código
git clone https://github.com/Coder-milo/Barbexa-barberia.git
cd Barbexa-barberia
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
El frontend se ejecutará en: http://localhost:5173

El backend en: http://localhost:3000

📡 Endpoints Principales
Auth
POST /api/v1/auth/register → Registro de usuario

POST /api/v1/auth/login → Inicio de sesión

Usuarios
GET /api/v1/users → Listar usuarios (solo admin)

GET /api/v1/users/:id → Obtener usuario por ID

Servicios
GET /api/v1/services → Listar servicios

POST /api/v1/services → Crear servicio (solo admin)

Reservas
GET /api/v1/bookings → Listar reservas

POST /api/v1/bookings → Crear reserva

🧪 Tests
En desarrollo. Se recomienda usar Jest para pruebas unitarias en backend y Vitest en frontend.

👨‍💻 Contribución
Haz un fork del repositorio.

Crea una nueva rama:

bash
Copiar código
git checkout -b feature/nueva-funcionalidad
Realiza tus cambios y haz commit:

bash
Copiar código
git commit -m "Agregada nueva funcionalidad"
Sube tu rama:

bash
Copiar código
git push origin feature/nueva-funcionalidad
Abre un Pull Request 🚀

📜 Licencia
Este proyecto está bajo la licencia MIT.
Puedes usarlo libremente con fines educativos y de desarrollo.

💡 Créditos
Desarrollado con ❤️ por:

Dalexa Sanjuan

José Camilo Doria

Sergio Bonilla

Sebastián Pineda

Juseth


