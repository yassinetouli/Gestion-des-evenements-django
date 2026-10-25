# Toul Events – Django Event Management System

A Django-based web application for creating, managing and tracking events.

---

## Table of Contents

1. [Overview](#overview)
2. [Features](#features)
3. [Project Structure](#project-structure)
4. [Tech Stack](#tech-stack)
5. [Getting Started (Local Development)](#getting-started-local-development)
6. [Deployment to Railway](#deployment-to-railway)
7. [Contributing](#contributing)
8. [Author](#author)

---

## Overview

**Toul Events** (repository: `Gestion-des-evenements-django`) is an event management system built with Django. It lets users create and manage events, with a dedicated dashboard and support for uploaded media (such as event images).

## Features

> Adjust this list to match the exact features implemented in your code.

- Full CRUD for events (create, read, update, delete) – `crud_event` app
- Dashboard for an overview of events – `dashboard` app
- Media uploads (event images and files) stored in `media/uploads`
- Email sending through SMTP
- Production-ready setup: static files collection, Docker, Procfile and Railway configuration

## Project Structure

```
Gestion-des-evenements-django/
├── gestion_des_evenements/   # Django project settings and configuration
├── main/                     # Main app (public pages)
├── crud_event/               # Event creation, listing, editing and deletion
│   ├── migrations/           # Database migrations
│   ├── templates/            # HTML templates for event pages
│   ├── __init__.py
│   ├── admin.py              # Django admin registration
│   ├── apps.py               # App configuration
│   ├── models.py             # Event data model
│   ├── urls.py               # App URL routes
│   ├── views.py              # CRUD views (create, list, update, delete)
│   └── tests.py              # Tests
├── dashboard/                # Dashboard app
├── media/uploads/            # User-uploaded files
├── staticfiles/              # Collected static files (collectstatic)
├── .vscode/                  # Editor settings
├── .env                      # Environment variables (see warning below)
```

## Tech Stack

| Layer          | Technology                                   |
| -------------- | -------------------------------------------- |
| Frontend         HTML, CSS(Tailwind)                          |
| Backend        | Python, Django                               |
| Database       | PostgreSQL (production on Railway)           |
| Deployment     | Railway (demo)                               |
| Email          | SMTP                                         |

## Getting Started (Local Development)

### Prerequisites

- Python (see `runtime.txt` for the exact version)
- Git
- pip (and optionally `venv`)

values, and rotate any exposed keys or passwords.

## Deployment to Railway

### Prerequisites

- A [Railway](https://railway.app) account
- Git installed locally
- Railway CLI (optional)

## Contributing

1. Fork the repository
2. Create a branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m "Add my feature"`
4. Push the branch: `git push origin feature/my-feature`
5. Open a Pull Request

## Author

**Yassine Touli** – [@yassinetouli](https://github.com/yassinetouli)
