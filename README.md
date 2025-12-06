# Learning Management System

Sistema completo de gestión de aprendizaje (LMS) desarrollado como aplicación full-stack para la administración de clases, evaluaciones, estudiantes y docentes.

## 📋 Descripción General

Este proyecto es una plataforma educativa que permite gestionar el ciclo completo de aprendizaje, desde la creación de clases y asignación de estudiantes, hasta la evaluación mediante exámenes y rúbricas. El sistema está diseñado para facilitar la administración académica con diferentes roles de usuario y funcionalidades especializadas.

### Funcionalidades Principales

- **Gestión de Usuarios**: Administración de estudiantes, docentes y administradores con roles diferenciados
- **Gestión de Clases**: Creación y administración de clases académicas con horarios y estudiantes asignados
- **Sistema de Evaluaciones**: Creación de exámenes y evaluaciones con diferentes tipos y criterios
- **Rúbricas**: Sistema de evaluación mediante rúbricas con criterios personalizables
- **Ciclos y Módulos Académicos**: Organización por ciclos académicos y módulos
- **Autenticación**: Sistema de autenticación con JWT y Google OAuth
- **Notificaciones**: Envío de correos electrónicos para notificaciones y recuperación de contraseña
- **Integración con Google Sheets**: Exportación e importación de datos mediante Google Sheets
- **Generación de QR**: Sistema de códigos QR para evaluaciones y clases

## 📁 Estructura del Proyecto

El proyecto está organizado en dos repositorios principales:

```
learning-full/
├── learning_front/          # Frontend - Aplicación React
│   └── README.md            # Documentación específica del frontend
│
└── learning_management/     # Backend - API REST con NestJS
    └── README.md            # Documentación específica del backend
```

### Frontend (`learning_front/`)

Aplicación web desarrollada con React, TypeScript y Vite que proporciona una interfaz de usuario moderna y responsive para interactuar con el sistema.

**Tecnologías principales:**
- React 19 + TypeScript
- Material-UI (MUI) + TailwindCSS
- React Router para navegación
- Zustand para gestión de estado
- Axios para comunicación con la API

### Backend (`learning_management/`)

API REST construida con NestJS que maneja toda la lógica de negocio, autenticación y persistencia de datos.

**Tecnologías principales:**
- NestJS (Framework Node.js)
- TypeORM + PostgreSQL
- Passport (JWT, Google OAuth)
- Swagger para documentación de API
- Nodemailer para envío de correos

## 🚀 Inicio Rápido

Para comenzar con el proyecto, cada repositorio tiene su propia documentación detallada con instrucciones específicas de instalación y configuración:

- **Frontend**: Consulta el `README.md` en `learning_front/` para instrucciones de configuración del frontend
- **Backend**: Consulta el `README.md` en `learning_management/` para instrucciones de configuración del backend, base de datos y migraciones

### Requisitos Generales

- **Node.js** >= 18
- **npm** >= 9
- **PostgreSQL** >= 13
- **Git**

### Pasos Básicos

1. Clonar el repositorio completo
2. Configurar el backend siguiendo las instrucciones en `learning_management/README.md`
3. Configurar el frontend siguiendo las instrucciones en `learning_front/README.md`
4. Iniciar ambos servidores

## 👥 Roles del Sistema

El sistema maneja tres roles principales con diferentes niveles de acceso:

- **Administrador**: Acceso completo al sistema, gestión de usuarios, ciclos académicos, carreras y configuración general
- **Docente**: Gestión de clases asignadas, creación de evaluaciones y rúbricas, visualización de resultados de estudiantes
- **Estudiante**: Visualización de clases asignadas, acceso a evaluaciones y visualización de resultados y calificaciones

## 🔐 Autenticación

El sistema soporta dos métodos de autenticación:

1. **Autenticación tradicional**: Email y contraseña con JWT
2. **Google OAuth**: Inicio de sesión con cuenta de Google

## 📚 Documentación

- **Backend API**: Documentación interactiva disponible en Swagger cuando el servidor está ejecutándose (`http://localhost:3001/api`)
- **Frontend**: Documentación específica en `learning_front/README.md`
- **Backend**: Documentación específica en `learning_management/README.md`
- **Base de Datos**: Scripts SQL de referencia en `learning_management/documentation/`

## 📦 Arquitectura

El proyecto sigue una arquitectura de separación de responsabilidades:

- **Frontend**: Interfaz de usuario y experiencia del usuario
- **Backend**: Lógica de negocio, validaciones y persistencia de datos
- **Base de Datos**: PostgreSQL con migraciones controladas mediante TypeORM

## 🧪 Testing

Cada repositorio incluye su propia suite de tests:

- **Backend**: Tests unitarios y e2e con Jest
- **Frontend**: Tests configurados según las mejores prácticas de React

## 🤝 Contribución

Para contribuir al proyecto:

1. Revisa la documentación específica de cada repositorio
2. Crea una rama nueva desde `main`
3. Realiza tus cambios siguiendo las convenciones del proyecto
4. Ejecuta los tests y el linter correspondientes
5. Crea un Pull Request con una descripción clara de los cambios

## 📄 Licencia

Este proyecto es privado y no tiene licencia pública.

---

**Nota**: Para instrucciones detalladas de instalación y configuración, consulta los archivos `README.md` específicos de cada repositorio (`learning_front/README.md` y `learning_management/README.md`).
