
# Cloud-Based Storage Service

A full-stack cloud storage and file sharing platform inspired by Google Drive, built with enterprise-grade architecture using Java Spring Boot and React.


## Overview

This application provides a secure, feature-rich file storage solution enabling users to upload, organize, search, and share files with fine-grained permission controls. Designed as an industry-ready MVP, it showcases modern full-stack development practices suitable for portfolio presentations and technical interviews.


## Key Features

### Core Functionality

- Secure Authentication (Email/Password, OAuth2, JWT)
- File Management (Upload, Download, Rename, Move, Soft Delete)
- Folder Organization with nested structure
- Smart Sharing with role-based permissions
- Public links with expiry and password protection
- Advanced Search with filters and pagination
- Starred Files
- Trash and Restore mechanism


## Future Enhancements

- File versioning
- In-browser preview for images and PDFs
- Activity logs and audit trails
- Custom tags and labels


## Architecture

### Technology Stack

#### Backend
- Java 17+
- Spring Boot
- Spring Security (JWT + OAuth2)
- Spring Data JPA with Hibernate
- Bean Validation
- RESTful APIs

#### Frontend
- React / Next.js
- Tailwind CSS
- TanStack Query
- Axios
- React Dropzone

#### Database and Storage
- PostgreSQL
- Supabase Storage

#### Deployment
- Frontend: Vercel / Netlify
- Backend: Render / Railway
- Database: Supabase

## System Design

[React Client]
      ↓
[Spring Boot REST API]
      ↓
[PostgreSQL] ↔ [S3 / Supabase Storage]


## Security Features

- JWT-based authentication
- OAuth2 integration
- Role-based access control
- Signed URLs
- Input validation
- Rate limiting



## Project Structure


backend/
frontend/


## Prerequisites

- Java 17+
- Node.js 18+
- PostgreSQL 14+
- Supabase account


## Backend Setup

cd backend
./mvnw clean install
./mvnw spring-boot:run



## Frontend Setup

cd frontend
npm install
npm run dev



## API Endpoints

### Authentication
- POST /api/auth/register
- POST /api/auth/login
- GET /api/auth/me

### File Operations
- POST /api/files/init-upload
- POST /api/files/complete-upload
- GET /api/files/{id}
- DELETE /api/files/{id}

### Folder Management
- POST /api/folders
- GET /api/folders/{id}

### Sharing
- POST /api/shares
- POST /api/public-links


## Skills Demonstrated

- Enterprise Java development
- RESTful API design
- JWT and OAuth2 authentication
- Cloud storage integration
- React frontend development
- Full-stack architecture

## License

Open source for educational and portfolio purposes.


Built with ❤️ using Java Spring Boot and React.
