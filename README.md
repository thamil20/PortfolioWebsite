# Portfolio Website

A full-stack portfolio website built with Django, React, and PostgreSQL.

## Project Structure

```
PortfolioWebsite/
├── backend/          # Django REST API
├── frontend/         # React application
└── README.md         # This file
```

## Quick Start

### Prerequisites

- Python 3.10+
- Node.js 16+
- PostgreSQL 12+
- Git

### Setup Instructions

#### 1. Backend Setup

1. Navigate to backend directory:
   ```bash
   cd backend
   ```

2. Create virtual environment:
   ```bash
   python -m venv venv
   ```

3. Activate virtual environment (Windows):
   ```bash
   venv\Scripts\activate
   ```
   
   Or on macOS/Linux:
   ```bash
   source venv/bin/activate
   ```

4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

5. Create `.env` file:
   ```bash
   copy .env.example .env
   ```
   
   Edit `.env` and configure your PostgreSQL credentials.

6. Create Django project and apps:
   ```bash
   django-admin startproject config .
   django-admin startapp users
   django-admin startapp portfolio
   django-admin startapp projects
   django-admin startapp blog
   ```

7. Configure Django settings (see `backend/README.md` for details)

8. Run migrations:
   ```bash
   python manage.py migrate
   ```

9. Create superuser:
   ```bash
   python manage.py createsuperuser
   ```

10. Run development server:
    ```bash
    python manage.py runserver
    ```

The API will be available at `http://localhost:8000`

#### 2. Frontend Setup

1. Navigate to frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create `.env` file:
   ```bash
   copy .env.example .env
   ```

4. Start development server:
   ```bash
   npm run dev
   ```

The app will be available at `http://localhost:3000`

## Development Workflow

### Phase 1: Authentication (Current)
- [x] Project structure
- [ ] Django user model and JWT authentication
- [ ] Django authentication endpoints
- [ ] React login/register pages
- [ ] Authentication context and state management

### Phase 2: Landing Page
- [ ] Skills model in Django
- [ ] Experience model in Django
- [ ] Frontend components for skills and experience
- [ ] API integration

### Phase 3: Projects Page
- [ ] Projects model
- [ ] Like functionality
- [ ] Project listing and detail pages
- [ ] Frontend integration

### Phase 4: Blog System
- [ ] Blog posts model
- [ ] Comments model
- [ ] Blog listing and detail pages
- [ ] Like and comment functionality

### Phase 5: Admin Dashboard
- [ ] Admin user role
- [ ] Admin dashboard layout
- [ ] Content management interfaces
- [ ] Statistics and analytics

## Technology Stack

### Backend
- **Django 4.2**: Web framework
- **Django REST Framework**: REST API toolkit
- **PostgreSQL**: Database
- **JWT**: Token-based authentication

### Frontend
- **React 18**: UI library
- **React Router v6**: Client-side routing
- **Axios**: HTTP client
- **Vite**: Build tool
- **Bootstrap 5**: CSS framework

## Documentation

- [Backend README](./backend/README.md) - Django setup and API details
- [Frontend README](./frontend/README.md) - React setup and component details

## Deployment

When ready for production, see the deployment guide (to be created).

## License

Add your license here.
