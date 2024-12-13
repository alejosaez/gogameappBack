# Backend Documentation

## **Application Name**
**Backend for GoGameApp**

## **Description**
This backend serves as the core API and real-time synchronization service for the GoGameApp. It provides a robust task management system using NestJS, a progressive Node.js framework, with SQLite as the database.

---

## **Key Features**
- **Task Management API**: Provides CRUD operations for managing tasks.
- **Real-time Updates**: Powered by WebSockets using `@nestjs/platform-socket.io`.
- **Database Integration**: Uses `TypeORM` for managing SQLite database operations.
- **Data Validation**: Implements validation using `class-validator` and `class-transformer`.
- **Modular Architecture**: Built with NestJS for maintainability and scalability.

---

## **Technologies Used**

### **Framework**
- **NestJS**: A Node.js framework for building efficient, reliable, and scalable server-side applications.

### **Database**
- **SQLite**: A lightweight relational database managed with `TypeORM`.

### **Real-Time Communication**
- **Socket.IO**: Enables real-time updates and communication for the application.

### **Validation**
- **class-validator**: Ensures data validation for API inputs.
- **class-transformer**: Provides serialization and transformation for DTOs.



## **System Requirements**
- **Node.js**: `>= 18`
- **NPM/Yarn**: Package manager for installing dependencies.

---

## **Project Structure**

```plaintext
src/
├── app.module.ts          # Root module of the application
├── main.ts                # Entry point of the application
├── tasks/                 # Task-related modules, controllers, and services
│   ├── tasks.controller.ts  # Handles HTTP requests for tasks
│   ├── tasks.service.ts     # Business logic for tasks
│   ├── tasks.module.ts      # Tasks module definition
│   ├── tasks.entity.ts      # TypeORM entity for tasks
├── websockets/            # WebSocket gateway for real-time updates
├── common/                # Shared modules, DTOs, and utilities
├── config/                # Application configuration
├── database/              # Database connection and migrations


## **Installation**

### **1. Clone the Repository**
```bash
git clone https://github.com/your-username/your-repository.git
cd backend

yarn install


## **Main Dependencies**

| Package                       | Version  | Description                              |
|-------------------------------|----------|------------------------------------------|
| `@nestjs/common`              | `^10.0.0`| Core NestJS functionality                |
| `@nestjs/core`                | `^10.0.0`| Application core                         |
| `@nestjs/platform-express`    | `^10.0.0`| Express platform integration             |
| `@nestjs/typeorm`             | `^10.0.2`| TypeORM integration for NestJS           |
| `@nestjs/platform-socket.io`  | `^10.4.15`| WebSocket platform for real-time updates |
| `typeorm`                     | `^0.3.20`| Database ORM                             |
| `sqlite3`                     | `^5.1.7` | SQLite database driver                   |


## **Development Tools**

| Package                       | Version  | Description                              |
|-------------------------------|----------|------------------------------------------|
| `typescript`                  | `^5.1.3`| Static typing                            |
| `eslint`                      | `^8.0.0`| Linting                                  |
| `prettier`                    | `^3.0.0`| Code formatting                          |
| `supertest`                   | `^7.0.0` | Integration testing for HTTP APIs        |


# Documentación del Backend

## **Nombre de la Aplicación**
**Backend para GoGameApp**

## **Descripción**
Este backend sirve como la API principal y el servicio de sincronización en tiempo real para la aplicación GoGameApp. Proporciona un sistema robusto de gestión de tareas utilizando NestJS, un framework progresivo de Node.js, con SQLite como base de datos.

---

## **Características Principales**
- **API de Gestión de Tareas**: Proporciona operaciones CRUD para gestionar tareas.
- **Actualizaciones en Tiempo Real**: Impulsado por WebSockets utilizando `@nestjs/platform-socket.io`.
- **Integración con la Base de Datos**: Usa `TypeORM` para gestionar las operaciones de la base de datos SQLite.
- **Validación de Datos**: Implementa validación utilizando `class-validator` y `class-transformer`.
- **Arquitectura Modular**: Construido con NestJS para facilitar el mantenimiento y escalabilidad.

---

## **Tecnologías Utilizadas**

### **Framework**
- **NestJS**: Un framework de Node.js para construir aplicaciones del lado del servidor eficientes, confiables y escalables.

### **Base de Datos**
- **SQLite**: Una base de datos relacional ligera gestionada con `TypeORM`.

### **Comunicación en Tiempo Real**
- **Socket.IO**: Permite actualizaciones y comunicación en tiempo real para la aplicación.

### **Validación**
- **class-validator**: Garantiza la validación de los datos para las entradas de la API.
- **class-transformer**: Proporciona serialización y transformación para los DTOs.


---

## **Requisitos del Sistema**
- **Node.js**: `>= 18`
- **NPM/Yarn**: Gestor de paquetes para instalar dependencias.

---

## **Estructura del Proyecto**

```plaintext
src/
├── app.module.ts          # Módulo raíz de la aplicación
├── main.ts                # Punto de entrada de la aplicación
├── tasks/                 # Módulos, controladores y servicios relacionados con tareas
│   ├── tasks.controller.ts  # Maneja las solicitudes HTTP para tareas
│   ├── tasks.service.ts     # Lógica de negocio para las tareas
│   ├── tasks.module.ts      # Definición del módulo de tareas
│   ├── tasks.entity.ts      # Entidad TypeORM para tareas
├── websockets/            # Puerta de enlace WebSocket para actualizaciones en tiempo real
├── common/                # Módulos compartidos, DTOs y utilidades
├── config/                # Configuración de la aplicación
├── database/              # Conexión y migraciones de la base de datos

Clonar el Repositorio
git clone https://github.com/your-username/your-repository.git
cd backend

## Instalar Dependencias

yarn install

## Variables de Entorno: Configura un archivo .env en el directorio raíz con las siguientes variables:

DATABASE_URL=sqlite:./database.sqlite

	Configuración de la Base de Datos:

  yarn typeorm migration:run

  ## Modo de Desarrollo:

  yarn start:prod

## **Dependencias Principales**

| Paquete                       | Versión  | Descripción                              |
|-------------------------------|----------|------------------------------------------|
| `@nestjs/common`              | `^10.0.0`| Funcionalidad central de NestJS          |
| `@nestjs/core`                | `^10.0.0`| Núcleo de la aplicación                  |
| `@nestjs/platform-express`    | `^10.0.0`| Integración con la plataforma Express    |
| `@nestjs/typeorm`             | `^10.0.2`| Integración con TypeORM para NestJS      |
| `@nestjs/platform-socket.io`  | `^10.4.15`| Plataforma WebSocket para actualizaciones en tiempo real |
| `typeorm`                     | `^0.3.20`| ORM para la base de datos                |
| `sqlite3`                     | `^5.1.7` | Controlador de base de datos SQLite      |

## ** Herramientas De Desarrollo**

| Paquete                       | Versión  | Descripción                              |
|-------------------------------|----------|------------------------------------------|
| `typescript`                  | `^5.1.3`| Tipado estático                          |
| `eslint`                      | `^8.0.0`| Linting                                  |
| `prettier`                    | `^3.0.0`| Formateo de código                       |                 |
| `supertest`                   | `^7.0.0` | Pruebas de integración para APIs HTTP    |
