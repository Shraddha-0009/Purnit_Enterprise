# 🏢 Purnit — Enterprise Workspace Platform

> A modern multi-role enterprise workspace platform designed to bring employees, HR teams, managers, and administrators together in a unified digital workspace.

## 📌 Overview

**Purnit** is an enterprise workspace platform designed to reduce dependency on multiple disconnected workplace applications by providing a centralized environment for managing employees, projects, meetings, notifications, workspaces, analytics, and organizational activities.

The platform follows a role-based architecture where different users receive access to features according to their responsibilities.

The project focuses on building a scalable foundation for an enterprise SaaS application with modern frontend technologies, reusable components, centralized state management, authentication, and backend integration.

---

## 🎯 Problem Statement

Modern organizations often use multiple applications for communication, project management, meetings, employee management, notifications, and analytics.

This can result in:

- Fragmented information
- Multiple application dependencies
- Difficult workflow management
- Repeated authentication
- Poor visibility across teams
- Increased administrative overhead

### Proposed Solution

Purnit provides a **unified enterprise workspace** where different organizational functions can be accessed from a single platform.

---

## ✨ Key Features

### 🔐 Authentication

- User registration
- User login
- Authentication state management
- Protected application routes
- Role-based access

### 👥 Role-Based Workspaces

The platform provides different interfaces for organizational roles such as:

- Administrator
- HR
- Employee
- Guest

This allows users to access features relevant to their responsibilities.

### 📊 Dashboard

The dashboard provides a centralized view of organizational activities and important information.

### 📁 Project Management

The project module provides an interface for managing organizational projects and tracking project-related information.

### 📅 Meeting Management

Users can access meeting-related functionality through a dedicated meetings module.

### 🔔 Notifications

A notification system is included to provide users with updates and application events.

### 📈 Analytics

The analytics section provides a foundation for visualizing organizational and workspace-related information.

### 👤 Profile & Settings

Users can manage profile-related information and application settings.

### 🌓 Theme Support

The platform supports:

- Light mode
- Dark mode
- System-based theme preference

### 🧩 Reusable UI Components

The application uses reusable components such as:

- Buttons
- Cards
- Tables
- Modals
- Dialogs
- Tabs
- Pagination
- Forms
- Tooltips
- Badges
- Loaders

This improves consistency and maintainability across the application.

---

## 🏗️ System Architecture

```text
                    ┌─────────────────────────┐
                    │        Purnit           │
                    │ Enterprise Workspace    │
                    └────────────┬────────────┘
                                 │
                    ┌────────────▼────────────┐
                    │      React Frontend     │
                    │     TypeScript + Vite   │
                    └────────────┬────────────┘
                                 │
             ┌───────────────────┼───────────────────┐
             │                   │                   │
             ▼                   ▼                   ▼
       Authentication       Workspace          Application
          & Roles           Management           Modules
             │                   │                   │
             │                   │        ┌──────────┼─────────┐
             │                   │        │          │         │
             ▼                   ▼        ▼          ▼         ▼
          Supabase          State       Projects   Meetings  Analytics
                            Management
                                 │
                                 ▼
                         Notifications
```

---

## 🛠️ Technology Stack

| Category | Technology |
|---|---|
| Frontend | React |
| Programming Language | TypeScript |
| Build Tool | Vite |
| Styling | Tailwind CSS |
| State Management | Zustand |
| Server State | TanStack Query |
| Routing | React Router |
| Backend / Database | Supabase |
| Forms | React Hook Form |
| Validation | Zod |
| Animations | Framer Motion |
| Icons | Lucide React |
| Charts | Recharts |
| Code Quality | ESLint |
| Formatting | Prettier |
| CI/CD | GitHub Actions |

---

## 🧱 Application Modules

```text
Purnit
│
├── Authentication
│   ├── Login
│   └── Registration
│
├── Workspace
│   ├── Dashboard
│   ├── Projects
│   ├── Meetings
│   ├── Analytics
│   └── Notifications
│
├── User Management
│   ├── Profile
│   └── Settings
│
├── Role-Based Layouts
│   ├── Admin
│   ├── HR
│   ├── Employee
│   └── Guest
│
└── UI System
    ├── Components
    ├── Themes
    ├── Modals
    ├── Tables
    └── Forms
```

---

## 🔐 Role-Based Access

Purnit follows a role-oriented architecture where application layouts and functionality can be controlled based on user roles and permissions.

Example:

```text
Administrator
      ↓
Administrative Workspace

HR
      ↓
HR Workspace

Employee
      ↓
Employee Workspace

Guest
      ↓
Limited Workspace
```

This architecture provides a foundation for implementing secure access control in an enterprise environment.

---

## ⚙️ Getting Started

### Prerequisites

Make sure the following are installed:

- Node.js 20+
- npm 10+
- Git

### Clone the repository

```bash
git clone <YOUR-GITHUB-REPOSITORY-URL>
cd Purnit_Enterprise
```

### Install dependencies

```bash
npm install
```

### Configure environment variables

Create a `.env` file based on the project's environment configuration.

Example:

```env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

Only add variables that are actually required by the application.

### Start development server

```bash
npm run dev
```

The application will normally be available at:

```text
http://localhost:5173
```

---

## 🔑 Backend Configuration

Purnit uses **Supabase** for backend-related functionality such as authentication and database integration.

To run the complete application, a properly configured Supabase project may be required.

The required environment variables should be placed in `.env`.

**Never commit private API keys, service-role keys, passwords, or other secrets to GitHub.**

---

## 📸 Screenshots

Add screenshots of the actual application here.

Recommended screenshots:

### Login

```text
screenshots/login.png
```

### Dashboard

```text
screenshots/dashboard.png
```

### Projects

```text
screenshots/projects.png
```

### Analytics

```text
screenshots/analytics.png
```

Example:

```markdown
![Dashboard](screenshots/dashboard.png)
```

---

## 🚀 Future Enhancements

- AI-powered enterprise assistant
- Intelligent document search
- RAG-based organizational knowledge system
- Automated meeting summaries
- AI-powered task recommendations
- Advanced workforce analytics
- Real-time collaboration
- Enhanced audit logging
- Advanced permission management
- Mobile application
- Cloud deployment
- Enterprise-grade monitoring

---

## 👩‍💻 Project Contribution

My contribution to the project includes work on the development and integration of the enterprise workspace platform, including:

- React and TypeScript development
- Reusable UI component development
- Role-based workspace interfaces
- Authentication and application flows
- Dashboard and module development
- Project and meeting interfaces
- State and service integration
- Responsive UI implementation
- Theme and user experience improvements

> Contribution details should be adjusted to accurately reflect the work personally completed by the project contributor.

---

## 📌 Project Status

**Status: Development / Working Prototype**

Purnit currently provides the foundation and interface for a multi-role enterprise workspace platform. Some modules and backend integrations may require additional configuration or implementation before production deployment.

---

## ⚠️ Disclaimer

This project is intended for educational, portfolio, and development purposes.

Production deployment requires proper backend configuration, authentication security, database rules, access-control policies, testing, monitoring, and secure management of environment variables.npx lint-staged
