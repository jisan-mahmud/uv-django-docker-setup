# Django uv Template

A production-ready Django project template leveraging uv for fast dependency management and Docker for containerized deployment.

## Overview

This template provides a modern Django development environment with industry best practices, optimized for rapid development and seamless deployment.

## Key Features

- **Fast Package Management**: uv for lightning-fast dependency resolution and installation
- **Modern Django Stack**: Django 6.0+ with Django REST Framework
- **Database Ready**: PostgreSQL integration with psycopg3
- **API Documentation**: Automated Swagger/OpenAPI docs via drf-spectacular
- **Production Optimized**: Gunicorn WSGI server and WhiteNoise static file serving
- **Containerized**: Docker support for development and production environments
- **Environment Management**: python-decouple for configuration management

## Quick Start

### Prerequisites
- Python 3.12+
- uv package manager
- Docker (optional)

### Local Development

```bash
# Clone and setup
git clone <repository-url>
cd uv-django

# Install dependencies
uv sync

# Database setup
uv run python manage.py migrate

# Start development server
uv run python manage.py runserver
```

### Docker Development

```bash
# Development environment
docker-compose -f docker-compose.local.yaml up --build

# Production environment
docker-compose up --build
```

## Technology Stack

- **Framework**: Django 6.0+
- **API**: Django REST Framework
- **Database**: PostgreSQL
- **Package Manager**: uv
- **Documentation**: drf-spectacular (Swagger/OpenAPI)
- **WSGI Server**: Gunicorn
- **Static Files**: WhiteNoise
- **Configuration**: python-decouple