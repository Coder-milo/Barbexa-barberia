# Barbexa - Backend API Documentation

## 📌 Project Overview
*Barbexa* is a *Node.js/Express backend API* for a barbershop management system.  
It provides endpoints for *services, reservations, combos, user management, and authentication*.  
The system integrates *role-based access control, **JWT authentication, and **MySQL database management*.


---

## 📂 Directory Structure


server/
├── src/
│   ├── config/        # Configuration files and DB setup
│   ├── controllers/   # Route handlers
│   ├── middlewares/   # Express middleware
│   ├── repositories/  # Database access layer
│   ├── routes/        # API route definitions
│   ├── services/      # Business logic layer
│   ├── shared/        # Utilities and helpers
│   └── doc/           # Documentation
├── .env               # Environment variables
├── app.js             # Express app setup
└── index.js           # Entry point

`

---

## ✨ Key Features
- 🔑 *JWT Authentication* with HTTP-only cookies  
- 🛡️ *Role-based access control* (Admin, Barber, Client)  
- 💈 *Service and combo management*  
- 📅 *Reservation system* with availability checking  
- 🗄️ *MySQL database* with connection pooling  
- ✅ Input validation and error handling  
- 🌐 *CORS configuration* for frontend integration  

---

## 📌 API Endpoints

### 🔑 Authentication
- POST /login → User login  
- POST /register → User registration  
- GET /profile → Get authenticated user profile  
- POST /logout → Logout user  

### 👤 Users
- GET /usersCount → Get total users count  
- GET /barberUser → Get all barbers  
- GET /users → Get all users  

### 💈 Services
- POST /services → Create service (*Admin only*)  
- GET /services → Get all active services  
- PUT /services/:id → Update service (*Admin only*)  
- DELETE /services/:id → Delete service (*Admin only*)  
- POST /barbers/:barberId/services → Assign services to a barber (*Admin only*)  

### 📅 Reservations
- POST /reservations → Create new reservation  
- GET /reservations/detail/:id → Get reservation details  
- GET /reservations/list → List reservations with filters  
- PATCH /reservations/:id/status → Update reservation status  
- GET /reservations/barber/:barberId/availability → Get barber availability  

### 🎁 Combos
- POST /combos → Create combo (*Admin only*)  
- GET /combos → Get all active combos  
- PUT /combos/:id → Update combo (*Admin only*)  
- DELETE /combos/:id → Delete combo (*Admin only*)  
- POST /combos/:id/services → Assign services to combo (*Admin only*)  

---

## ⚙️ Setup & Installation

### 1. Clone repository
bash
git clone <repo_url>
cd server
`

### 2. Install dependencies

bash
npm install


### 3. Configure environment variables (.env)

env
PORT=3000
DB_HOST=localhost
DB_USER=user
DB_PASSWORD=password 
DB_NAME=barbexa
DB_PORT=3306
JWT_SECRET=secret
JWT_EXPIRES=1h


### 4. Initialize database

bash
mysql -u root -p < src/doc/script.sql


### 5. Run the server

* Development (hot reload):

bash
npm run dev


* Production:

bash
npm start


---

## 🗄️ Database Schema

The database includes the following tables:

* *Users & Roles*
* *Services*
* *Reservations*
* *Service Combos*
* *Barber Availability*
* Relationship tables

➡️ See src/doc/script.sql for full schema.

---

## 🔒 Security

* Password hashing with *bcrypt*
* JWT stored in *HTTP-only cookies*
* Role-based access control
* Input validation
* CORS configuration
* Global error handling

---

## 🛠️ Development Stack

* [Node.js](https://nodejs.org/) & [Express](https://expressjs.com/)
* [MySQL](https://www.mysql.com/) with mysql2/promise
* [JWT](https://jwt.io/) for authentication
* [bcrypt](https://github.com/kelektiv/node.bcrypt.js) for password hashing
* [dayjs](https://day.js.org/) for date/time handling
* [dotenv](https://github.com/motdotla/dotenv) for configuration

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to branch
5. Open a Pull Request

---

## 📄 License

Licensed under the *ISC License*.
See [LICENSE](./LICENSE) for details.

```
