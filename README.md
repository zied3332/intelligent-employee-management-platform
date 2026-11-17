
# Intelligent Employee Management Platform

A production-style full-stack HR management platform developed as part of the **Engineering Program at ESPRIT School of Engineering (2025–2026)**.

The platform enables HR teams, managers, and employees to efficiently manage organizational data, streamline HR workflows, monitor employee activities, and leverage AI-powered recommendations for smarter workforce management.

Built using **React, TypeScript, NestJS, MongoDB, Python, FastAPI, and Scikit-learn**, the project demonstrates a modular architecture integrating modern web technologies with machine learning.

---

## Overview

The Intelligent Employee Management Platform is a collaborative software engineering project designed to simplify and improve human resource management.

The system follows a modular architecture composed of three independent services:

- **Frontend:** React application providing responsive, role-based dashboards and user interfaces.
- **Backend:** NestJS REST API responsible for authentication, authorization, business logic, and data management.
- **AI Service:** FastAPI microservice providing intelligent employee recommendations, similarity analysis, and machine learning capabilities.

These services work together to deliver a scalable and maintainable HR management solution.

---

## Project Repositories

The project is organized into three separate GitHub repositories.

| Component | Repository | Description |
|-----------|------------|-------------|
| Frontend | [4TWIN2-2026-WeebGeeks-FrontEnd](https://github.com/zied3332/4TWIN2-2026-WeebGeeks-FrontEnd) | React + TypeScript application with responsive dashboards for HR, Managers, and Employees |
| Backend | [Esprit-PIDEV-4TWIN2-2026-WeebGeeks](https://github.com/Malek-Fridhi/Esprit-PIDEV-4TWIN2-2026-WeebGeeks) | NestJS REST API with JWT authentication, MongoDB, role-based access control, and business logic |
| AI Service | [4TWIN2-2026-WeebGeeks-AI](https://github.com/zied3332/4TWIN2-2026-WeebGeeks-AI) | FastAPI microservice providing employee similarity, clustering, and recommendation services |

---

## Features

### Authentication & Security

- JWT-based authentication
- Role-Based Access Control (RBAC)
- HR, Manager, and Employee roles
- Protected API endpoints
- Authentication middleware and guards
- Secure REST API communication

### Employee Management

- Employee profile management
- Department management
- User administration
- Team management
- Employee directory
- Employee information management

### Activity Management

- Employee activity tracking
- Activity history
- Team collaboration
- Performance monitoring
- Activity management workflows

### AI-Powered Features

- Intelligent employee recommendation system
- Employee similarity search
- Clustering-based employee segmentation
- Machine learning integration
- Intelligent recruitment assistance
- Data-driven employee analysis

### Additional Utilities

- Excel import and export
- Responsive dashboards
- RESTful API architecture
- Modular service architecture
- Role-specific user interfaces
- Structured data management

---

## Tech Stack

### Frontend

| Technology | Purpose |
|------------|---------|
| React | User interface development |
| TypeScript | Type-safe application development |
| Vite | Development server and build tooling |
| React Router | Client-side routing |
| Material UI | UI components |
| Tailwind CSS | Responsive styling |
| Axios | HTTP requests and API integration |

### Backend

| Technology | Purpose |
|------------|---------|
| NestJS | Backend application framework |
| TypeScript | Server-side development |
| MongoDB | NoSQL database |
| Mongoose | MongoDB object modeling |
| JWT | Authentication |
| REST API | Communication between services |
| Docker | Containerization |

### AI Service

| Technology | Purpose |
|------------|---------|
| Python | Machine learning development |
| FastAPI | AI microservice REST API |
| Scikit-learn | Machine learning algorithms |
| Pandas | Data processing and analysis |
| NumPy | Numerical computing |
| Jupyter Notebook | Model experimentation |

---

## System Architecture

The platform uses a modular architecture that separates the user interface, business logic, database, and artificial intelligence components.

```text
                  +--------------------------+
                  |                          |
                  |      React Frontend      |
                  |    TypeScript + Vite     |
                  |                          |
                  +------------+-------------+
                               |
                               | HTTP / REST API
                               |
                  +------------v-------------+
                  |                          |
                  |      NestJS Backend      |
                  |                          |
                  |  Authentication + RBAC   |
                  |     Business Logic       |
                  |                          |
                  +------------+-------------+
                               |
                +--------------+--------------+
                |                             |
                |                             |
     +----------v----------+       +----------v----------+
     |                     |       |                     |
     |       MongoDB       |       |   FastAPI Service   |
     |                     |       |                     |
     |   Employee Data     |       |  Employee Analysis  |
     |   Departments       |       |  Recommendations    |
     |   Activities        |       |  Similarity Search  |
     |                     |       |                     |
     +---------------------+       +----------+----------+
                                              |
                                   +----------v----------+
                                   |                     |
                                   |  Machine Learning   |
                                   |                     |
                                   |   Scikit-learn      |
                                   |   Pandas / NumPy    |
                                   |   Clustering        |
                                   |                     |
                                   +---------------------+
```

### Communication Flow

1. Users interact with the React frontend.
2. The frontend sends HTTP requests to the NestJS backend.
3. The backend validates authentication and authorization.
4. Business logic processes requests and accesses MongoDB.
5. AI-related operations are delegated to the FastAPI microservice.
6. Machine learning models process employee information.
7. Results are returned through the backend to the frontend.

This separation allows each service to be developed, maintained, and extended independently.

---

## Repository Structure

The application is divided into three independent projects.

```text
Intelligent-Employee-Management-Platform/
|
+-- Frontend/
|   |
|   +-- React
|   +-- TypeScript
|   +-- Vite
|   +-- React Router
|   +-- Material UI
|   +-- Tailwind CSS
|   +-- Axios
|
+-- Backend/
|   |
|   +-- NestJS
|   +-- TypeScript
|   +-- MongoDB
|   +-- Mongoose
|   +-- JWT Authentication
|   +-- REST API
|   +-- Docker
|
+-- AI-Service/
    |
    +-- Python
    +-- FastAPI
    +-- Scikit-learn
    +-- Pandas
    +-- NumPy
    +-- Jupyter Notebook
    +-- Machine Learning Models
```

Each component is maintained in its own GitHub repository.

---

## AI & Machine Learning

The AI microservice extends traditional HR management functionality with intelligent workforce analysis.

### Employee Recommendation System

Analyzes employee information to generate recommendations based on relevant attributes and similarity patterns.

### Employee Similarity Search

Identifies employees with similar characteristics using machine learning techniques.

Potential applications include:

- Employee matching
- Team composition assistance
- Talent discovery
- Workforce analysis

### Employee Clustering

Uses unsupervised machine learning to group employees based on shared characteristics.

This enables HR teams to explore workforce segments and identify patterns within employee data.

### Intelligent Recruitment Assistance

Supports recruitment-related analysis through data-driven recommendations and employee matching techniques.

### AI Integration Workflow

```text
Employee Data
      |
      v
Data Preprocessing
      |
      v
Feature Extraction
      |
      v
Machine Learning Models
      |
      +----------------------+
      |                      |
      v                      v
Similarity Analysis     Clustering
      |                      |
      +-----------+----------+
                  |
                  v
        Recommendation Engine
                  |
                  v
           FastAPI REST API
                  |
                  v
            NestJS Backend
                  |
                  v
            React Frontend
```

---

## Security Architecture

The platform implements role-based security to control access to sensitive organizational information.

### Authentication

JWT authentication is used to identify authenticated users and secure API requests.

### Authorization

Role-Based Access Control restricts access to features based on user responsibilities.

| Role | Main Responsibilities |
|------|-----------------------|
| HR | Employee administration, organizational management, and workforce monitoring |
| Manager | Team management, employee activities, and performance monitoring |
| Employee | Personal profile access and assigned activity management |

### API Protection

Protected routes and authentication guards help prevent unauthorized access to restricted resources.

---

## Development Approach

The project follows a collaborative, modular development approach.

### Separation of Concerns

Each service has a dedicated responsibility:

- Frontend handles presentation and user interaction.
- Backend handles business logic, authentication, and persistence.
- AI service handles machine learning and intelligent analysis.

### Team Collaboration

Development was coordinated using Git and GitHub, allowing contributors to work on different modules and services.

### Maintainability

The modular architecture supports independent updates, testing, and future feature extensions.

---

## Learning Outcomes

This project demonstrates practical experience with:

- Full-stack web application development
- REST API design and implementation
- Authentication and authorization
- Role-Based Access Control
- Modular software architecture
- Microservice integration
- AI service development
- Machine learning workflows
- Employee similarity analysis
- Clustering algorithms
- MongoDB database design
- Responsive user interface development
- Git and GitHub collaboration
- Integration between multiple technology stacks

---

## Academic Context

This project was developed during the **2025–2026 academic year** as part of the Engineering Program at **ESPRIT School of Engineering, Tunisia**.

The objective was to design and implement a complete software engineering solution combining:

- Modern frontend technologies
- Scalable backend development
- Database management
- Secure authentication
- Artificial intelligence
- Collaborative software development

The project demonstrates the integration of traditional enterprise application development with AI-powered decision-support capabilities.

---

## Contributors

Developed collaboratively by the **WeebGeeks** team.

- **Zied Alimi**
- **Ahlem Bounasri**
- **Yasmine Ben Abdelali**
- **Malek Fridhi**
- **Mohamed Nour Slimi**

---

## Project Links

**Frontend Repository**

https://github.com/zied3332/4TWIN2-2026-WeebGeeks-FrontEnd

**Backend Repository**

https://github.com/Malek-Fridhi/Esprit-PIDEV-4TWIN2-2026-WeebGeeks

**AI Service Repository**

https://github.com/zied3332/4TWIN2-2026-WeebGeeks-AI

---

## License

This repository is provided for educational, academic, and portfolio purposes.

No specific open-source license is declared unless a separate LICENSE file is provided.

---

**Intelligent Employee Management Platform — WeebGeeks | ESPRIT School of Engineering | 2025–2026**
