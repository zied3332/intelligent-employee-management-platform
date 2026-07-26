# Intelligent Employee Management Platform

A production-style full-stack HR management platform developed as part of the Engineering Program at Esprit School of Engineering (2025–2026).

The platform enables HR teams, managers, and employees to efficiently manage organizational data, track activities, and leverage AI-powered recommendations for smarter workforce management.

---

## Project Architecture

This project is organized into three independent repositories:

| Repository | Description |
|------------|-------------|
| Frontend | React + TypeScript application |
| Backend | NestJS REST API |
| AI Service | FastAPI service providing machine learning features |

---

## Features

### Authentication & Authorization

- JWT Authentication
- Role-Based Access Control (HR, Manager, Employee)
- Secure API communication

### Employee Management

- Employee profiles
- Team management
- Department management
- User administration

### Activity Management

- Activity tracking
- Employee history
- Team collaboration

### AI Features

- Employee recommendation system
- Similar employee search
- Clustering-based analysis
- Machine learning services

### Utilities

- Excel import/export
- Responsive dashboards
- RESTful API architecture

---

## Tech Stack

### Frontend

- React
- TypeScript
- Vite
- React Router
- Material UI
- Tailwind CSS
- Axios

### Backend

- NestJS
- MongoDB
- Mongoose
- JWT Authentication
- REST API

### AI Service

- Python
- FastAPI
- Scikit-learn
- Pandas
- NumPy

---

## System Architecture

```text
                React Frontend
                       │
                       │ REST API
                       ▼
              NestJS Backend API
                 │           │
                 │           │
                 ▼           ▼
            MongoDB      FastAPI AI Service
                               │
                               ▼
                     Machine Learning Models
```

---

## Learning Objectives

This project demonstrates experience with:

- Full-stack web development
- REST API design
- Authentication & Authorization
- AI service integration
- Modular backend architecture
- Team collaboration using Git
- Responsive UI development
- Machine learning integration

---

## Academic Context

Developed during the Engineering Program at **Esprit School of Engineering** (Tunisia) as a collaborative software engineering project.

---

## Contributors

- Zied Alimi
- Ahlem Bounasri
- Yasmine Ben Abdelali
- Malek Fridhi
- Mohamed Nour Slimi
