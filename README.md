# Intelligent Employee Management Platform

A production-style full-stack HR management platform developed as part of the Engineering Program at **Esprit School of Engineering** (2025–2026).

The platform enables HR teams, managers, and employees to efficiently manage organizational data, streamline HR workflows, monitor employee activities, and leverage AI-powered recommendations for smarter workforce management.

---

## Overview

The system follows a modular architecture composed of three independent services:

- **Frontend** – React application providing role-based dashboards and user interfaces.
- **Backend** – NestJS REST API responsible for authentication, business logic, and data management.
- **AI Service** – FastAPI microservice providing intelligent employee recommendations and machine learning capabilities.

---

# Project Repositories

| Component | Repository | Description |
|-----------|------------|-------------|
| Frontend | https://github.com/YOUR_USERNAME/frontend-repository | React + TypeScript application with responsive dashboards for HR, Managers, and Employees |
| Backend | https://github.com/YOUR_USERNAME/backend-repository | NestJS REST API with JWT authentication, MongoDB, RBAC, and business logic |
| AI Service | https://github.com/YOUR_USERNAME/ai-repository | FastAPI microservice providing employee similarity, clustering, and recommendation services |

---

# Features

## Authentication & Security

- JWT Authentication
- Role-Based Access Control (HR, Manager, Employee)
- Secure REST API
- Protected routes
- Authentication middleware

---

## Employee Management

- Employee profile management
- Department management
- User administration
- Team management
- Employee directory

---

## Activity Management

- Employee activity tracking
- Activity history
- Team collaboration
- Performance monitoring

---

## AI Features

- Employee recommendation system
- Employee similarity search
- Clustering-based employee segmentation
- Machine learning integration
- Intelligent recruitment assistance

---

## Utilities

- Excel import/export
- Responsive dashboards
- RESTful API architecture
- Modular service architecture

---

# Tech Stack

## Frontend

- React
- TypeScript
- Vite
- React Router
- Material UI
- Tailwind CSS
- Axios

---

## Backend

- NestJS
- MongoDB
- Mongoose
- JWT Authentication
- REST API
- Docker

---

## AI Service

- Python
- FastAPI
- Scikit-learn
- Pandas
- NumPy
- Jupyter Notebook

---

# System Architecture

```text
                     +-----------------------+
                     |   React Frontend      |
                     +-----------+-----------+
                                 |
                                 | REST API
                                 |
                     +-----------v-----------+
                     |    NestJS Backend     |
                     +-----------+-----------+
                                 |
                  +--------------+--------------+
                  |                             |
                  |                             |
        +---------v---------+        +----------v----------+
        |     MongoDB       |        |  FastAPI AI Service |
        +-------------------+        +----------+----------+
                                                |
                                                |
                                       Machine Learning
                                            Models
```

---

# Repository Structure

```
Intelligent Employee Management Platform
│
├── Frontend
│   ├── React
│   ├── TypeScript
│   ├── Material UI
│   └── Tailwind CSS
│
├── Backend
│   ├── NestJS
│   ├── MongoDB
│   ├── JWT Authentication
│   └── REST API
│
└── AI Service
    ├── FastAPI
    ├── Scikit-learn
    ├── Pandas
    ├── NumPy
    └── Machine Learning Models
```

---

# Learning Outcomes

This project demonstrates practical experience with:

- Full-stack web development
- REST API development
- Authentication & Authorization
- Role-Based Access Control
- Modular software architecture
- AI service integration
- Machine learning workflows
- Database design
- Responsive UI development
- Team collaboration using Git

---

# Academic Context

This project was developed during the **Engineering Program at Esprit School of Engineering (Tunisia)** as a collaborative software engineering project.

---

# Contributors

- Zied Alimi
- Ahlem Bounasri
- Yasmine Ben Abdelali
- Malek Fridhi
- Mohamed Nour Slimi

---

# License

This repository is provided for educational and portfolio purposes.
