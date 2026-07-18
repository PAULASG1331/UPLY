# 📚 UPLY - Student Dashboard Platform

Plataforma educativa completa para gestionar tareas, clases, horarios y tutorías de estudiantes.

## 🎯 Características Principales

### ✅ Funcionalidades Implementadas
- **Dashboard Interactivo** - Panel principal con estadísticas en tiempo real
- **Autenticación de Usuarios** - Login y registro seguro
- **Gestión de Tareas** - Crear, editar y organizar tareas por estado
- **Horario Semanal** - Calendario de clases y eventos
- **Clases en Vivo** - Videoconferencias con profesores
- **Panel de Tutores** - Directorio de tutores disponibles
- **Perfil de Usuario** - Configuración y preferencias personales

## 🛠️ Tecnologías Utilizadas

- **Frontend**: React 18, CSS3, JavaScript ES6+
- **Backend**: Node.js, Express.js (preparado)
- **Base de Datos**: MongoDB (preparado)
- **Autenticación**: JWT (JSON Web Tokens)
- **Comunicación**: Fetch API, REST

## 📁 Estructura del Proyecto

```
UPLY/
├── index.html                 # App principal
├── pages/
│   ├── login.html            # Página de autenticación
│   ├── lessons.html          # Clases y tutores
│   ├── timetable.html        # Horario
│   └── homework.html         # Gestión de tareas
├── js/
│   ├── auth.js               # Sistema de autenticación
│   ├── api.js                # Conexión con backend
│   └── utils.js              # Funciones auxiliares
├── css/
│   └── styles.css            # Estilos compartidos
├── backend/
│   ├── server.js             # Servidor Express
│   ├── models/               # Modelos de datos
│   ├── routes/               # Rutas API
│   └── middleware/           # Middleware personalizado
└── README.md                 # Este archivo
```

## 🚀 Instalación y Configuración

### Frontend (Local)
```bash
# Clonar repositorio
git clone https://github.com/PAULASG1331/UPLY.git
cd UPLY

# Abrir en navegador
open index.html
# o
xdg-open index.html  # Linux
```

### Backend (Node.js)
```bash
cd backend
npm install
npm start
```

## 🔐 Autenticación

La aplicación incluye:
- **Registro de nuevos usuarios**
- **Login con email y contraseña**
- **Tokens JWT para sesiones seguras**
- **Recuperación de contraseña**
- **Cierre de sesión seguro**

## 📊 Endpoints API (Backend)

```
POST   /api/auth/register      - Registrar usuario
POST   /api/auth/login         - Iniciar sesión
POST   /api/auth/logout        - Cerrar sesión
GET    /api/users/profile      - Obtener perfil
PUT    /api/users/profile      - Actualizar perfil
GET    /api/tasks              - Listar tareas
POST   /api/tasks              - Crear tarea
PUT    /api/tasks/:id          - Editar tarea
DELETE /api/tasks/:id          - Eliminar tarea
GET    /api/lessons            - Listar clases
GET    /api/tutors             - Listar tutores
```

## 🎓 Casos de Uso

1. **Estudiante se registra** → Crea cuenta con email
2. **Inicia sesión** → Accede al dashboard
3. **Ve sus tareas** → Organiza por deadline
4. **Consulta horario** → Ve clases disponibles
5. **Se conecta a clase viva** → Videoconferencia con tutor
6. **Actualiza perfil** → Guarda preferencias

## 🔗 Integración de Datos

### Conexión Base de Datos MongoDB
```javascript
// Configuración en backend
const MONGODB_URI = "mongodb+srv://user:pass@cluster.mongodb.net/uply";
```

### Sincronización en Tiempo Real
- Datos se actualizan automáticamente
- Notificaciones push para nuevas tareas
- Estado compartido entre pestañas

## 📱 Responsive Design

- ✅ Desktop (1440px+)
- ✅ Tablets (768px - 1024px)
- ✅ Mobile (< 768px)

## 🔒 Seguridad

- Tokens JWT con expiración
- CORS habilitado
- Validación de entrada
- Encriptación de contraseñas
- HTTPS recomendado

## 📝 Licencia

Este proyecto es parte del servicio educativo UPLY.

## 👥 Soporte

- 📧 Email: support@uply.edu
- 💬 Chat: Available 24/7
- 📞 Teléfono: +1-XXX-XXX-XXXX

---

**Versión**: 1.0.0  
**Última actualización**: Julio 2026
