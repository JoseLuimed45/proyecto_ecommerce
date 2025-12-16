
# Proyecto Ecommerce

## Integrantes del Grupo de Desarrollo
- José Luis Medina
- Alejandro Placencia

## Funcionalidades Principales
- Autenticación de usuarios (registro, login, JWT)
- Gestión de productos (CRUD)
- Gestión de órdenes de compra
- Administración de usuarios y roles
- Registro de logs y auditoría
- Integración con servicios externos (Cloudinary, MongoDB)
- Pruebas unitarias y de integración

## Endpoints Utilizados

### Autenticación
- `POST /api/auth/login` — Inicio de sesión
- `POST /api/auth/register` — Registro de usuario

### Productos
- `GET /api/products` — Listar productos
- `POST /api/products` — Crear producto
- `PUT /api/products/:id` — Actualizar producto
- `DELETE /api/products/:id` — Eliminar producto

### Órdenes
- `GET /api/orders` — Listar órdenes
- `POST /api/orders` — Crear orden

### Administración
- `GET /api/admin/users` — Listar usuarios
- `POST /api/admin/users` — Crear usuario
- `PUT /api/admin/users/:id` — Actualizar usuario
- `DELETE /api/admin/users/:id` — Eliminar usuario

### Salud y utilidades
- `GET /api/health` — Verificar estado del backend

## Pasos para Ejecutar la Aplicación

### 1. Clonar el repositorio
```bash
git clone https://github.com/JoseLuimed45/proyecto_ecommerce.git
cd proyecto_ecommerce
```

### 2. Configurar variables de entorno
- Revisar y completar los archivos `.env` o `local.properties` según corresponda para backend y frontend.

### 3. Instalar dependencias
#### Backend
```bash
cd BackendAjicolor
npm install
```
#### Frontend (Android)
```bash
cd Ajicolor
./gradlew build
```

### 4. Ejecutar la aplicación
#### Backend
```bash
cd BackendAjicolor
npm start
```
#### Frontend (Android)
- Abrir el proyecto en Android Studio y ejecutar en un emulador o dispositivo físico.

### 5. Ejecutar pruebas unitarias
#### Backend
```bash
cd BackendAjicolor
npm test
```
#### Frontend (Android)
```bash
cd Ajicolor
./gradlew test
```

## Estructura Resumida del Proyecto

```
proyecto_ecommerce/
│
├── Ajicolor/                # Aplicación Android
│   ├── app/
│   ├── build.gradle.kts
│   └── ...
│
├── BackendAjicolor/         # Backend Node.js
│   ├── src/
│   │   ├── controllers/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── routes/
│   │   └── utils/
│   ├── package.json
│   └── ...
│
└── FimasJKS/                # Archivos de firma
```

---

Este README resume las funcionalidades, endpoints, pasos de ejecución, pruebas y estructura del proyecto para fines de auditoría.
