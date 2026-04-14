# 🔗 URL Shortener (Full Stack Backend)

A production-ready URL Shortener built using NestJS, PostgreSQL, JWT Authentication, and Docker.

---

## 🚀 Features

* 🔐 JWT Authentication (Signup & Login)
* 🔗 Shorten long URLs into unique short links
* 🔁 Redirect short URLs to original links
* 📊 Track visit analytics (click count)
* 🐳 Fully Dockerized for easy deployment
* 📄 Swagger API documentation

---

## 🛠️ Tech Stack

* Backend: NestJS (Node.js)
* Database: PostgreSQL
* Authentication: JWT + Bcrypt
* Deployment: Docker & Docker Compose

---

## 📂 API Endpoints

### Auth

* POST `/v1/auth/sign-up`
* POST `/v1/auth/sign-in`

### URL

* POST `/v1/urls/shorten`
* GET `/v1/urls/:shortUrl`
* GET `/v1/urls/stats/:shortUrl`

---

## ⚙️ Setup Instructions

```bash
git clone https://github.com/Mm240/url-shortener.git
cd url-shortener
docker-compose up --build -d
```

---

## 📊 Example Usage

### 1. Sign Up

```json
{
  "email": "user@example.com",
  "password": "Password123!",
  "confirmPassword": "Password123!"
}
```

### 2. Shorten URL

```json
{
  "originalUrl": "https://google.com"
}
```

---

## 🌐 API Docs

Access Swagger UI:

```
http://localhost:4000/api-docs
```

---

## 💼 Resume Highlights

* Built scalable URL shortener using NestJS and PostgreSQL
* Implemented JWT authentication and secure password hashing
* Designed REST APIs with analytics tracking
* Containerized application using Docker

---

## 👨‍💻 Contributors

* Maulik Mittal
* Manya

---

## ⭐ Future Improvements

* React Frontend UI
* Custom short URLs
* Rate limiting & caching
* Deployment on cloud (Render / Railway)
