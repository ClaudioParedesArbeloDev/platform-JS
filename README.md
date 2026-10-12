<h1 align="center">Code & Lens · Plataforma educativa (v1 · MERN)</h1>

<p align="center">
  Plataforma de cursos con chat en tiempo real, hecha con MongoDB, Express, React y Node · Course platform with real-time chat built on the MERN stack
</p>

<p align="center">
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" />
  <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Socket.io-010101?style=for-the-badge&logo=socketdotio&logoColor=white" />
  <img src="https://img.shields.io/badge/Sass-CC6699?style=for-the-badge&logo=sass&logoColor=white" />
</p>

<p align="center">
  <a href="#-español">Español</a> · <a href="#-english">English</a>
</p>

> 📌 **Primera versión** de la plataforma de Code & Lens. Luego migrada a Laravel: **[platform-Laravel](https://github.com/ClaudioParedesArbeloDev/platform-Laravel)** → **[platform-laravel-taildwind](https://github.com/ClaudioParedesArbeloDev/platform-laravel-taildwind)** (actual).

---

## 🇪🇸 Español

### Qué es

Plataforma educativa full stack: los alumnos se registran, acceden a cursos y su contenido, y conversan en un **chat en tiempo real** con Socket.io. Incluye un panel para gestionar usuarios y cursos.

### Funcionalidades

- Registro y login con **JWT** en cookie y sesiones guardadas en MongoDB (`connect-mongo`).
- Contraseñas hasheadas con bcrypt y recuperación de contraseña por email (**Nodemailer**).
- ABM de usuarios y cursos; carga de contenidos por curso.
- Subida de imágenes con Multer y optimización con **Sharp**.
- **Chat en vivo** con historial de mensajes persistido.
- Frontend en React (React Router) con estilos en Sass.

### Estructura

```
platform-JS/
├── index.js           # servidor HTTP + Socket.io + conexión a MongoDB
├── app.js             # app Express (middlewares y rutas)
├── src/
│   ├── controllers/   # auth, cursos, usuarios, mail
│   ├── models/        # Mongoose: usuarios, cursos, contenidos, chat
│   ├── middlewares/   # validación de token
│   └── libs/          # helpers JWT
└── public/            # frontend React
```

### Instalación

```bash
git clone https://github.com/ClaudioParedesArbeloDev/platform-JS.git
cd platform-JS
npm install
# crear .env con la URI de MongoDB, secreto JWT y datos SMTP
node index.js

# Frontend
cd public
npm install
npm start
```

---

## 🇬🇧 English

### What it is

Full stack learning platform: students sign up, access courses and their content, and talk in a **real-time chat** powered by Socket.io. Includes a panel to manage users and courses.

### Features

- Sign-up/login with **JWT** in cookies and MongoDB-backed sessions.
- bcrypt password hashing and email password reset (**Nodemailer**).
- User and course CRUD; per-course content upload.
- Image upload with Multer and optimisation with **Sharp**.
- **Live chat** with persisted message history.
- React (React Router) frontend styled with Sass.

### Setup

```bash
npm install
# create .env with MongoDB URI, JWT secret and SMTP settings
node index.js
cd public && npm install && npm start
```

---

<p align="center">
  Hecho por / Built by <a href="https://github.com/ClaudioParedesArbeloDev"><b>Claudio Paredes Arbelo</b></a> · <a href="https://www.claudioparedes.site">Code & Lens Solutions</a>
</p>
# Study Platform

Welcome to the Study Platform! This is a full-stack application designed to enhance interactive learning, featuring a frontend built with **React.js**, a backend powered by **Express.js**, real-time chat using **WebSockets**, modern styling with **Sass**, and data storage with **MongoDB**.

## Description

This platform enables users to access educational content, collaborate with peers via real-time chat, and manage their learning experience. It’s a dynamic and user-friendly solution built with modern technologies.

## Technologies Used

- **Frontend**: React.js - Dynamic UI with reusable components.
- **Backend**: Express.js - RESTful API for server-side logic.
- **Real-Time Chat**: WebSockets - Instant bidirectional communication.
- **Styling**: Sass - Modular and maintainable CSS preprocessing.
- **Database**: MongoDB - Flexible NoSQL database for scalable data management.

## Features

- Intuitive and responsive user interface.
- Real-time chat for seamless user interaction.
- User authentication and course management.

## Installation

Follow these steps to set up the project locally:

### Prerequisites
- Node.js (recommended version: 16.x or higher)
- MongoDB (installed locally or connected via a service like MongoDB Atlas)
- Git

