Sistema de Reservas para Restaurante
📋 Descripción del Proyecto
Sistema completo de gestión de reservas para restaurantes con interfaz para clientes y meseros.
🛠️ Stack Tecnológico
Backend

Django: Framework web robusto y maduro
Django REST Framework: Para crear APIs REST potentes
SQLite: Base de datos por defecto de Django

Frontend

React: Biblioteca de JavaScript para interfaces de usuario
Vite: Herramienta de desarrollo rápida
Axios: Cliente HTTP para consumir la API

📁 Estructura del Proyecto
sistema-reservas-restaurante/
├── backend/
│   ├── restaurant_reservations/
│   │   ├── settings.py
│   │   ├── urls.py
│   │   └── wsgi.py
│   ├── reservas/
│   │   ├── models.py
│   │   ├── views.py
│   │   ├── serializers.py
│   │   └── urls.py
│   ├── requirements.txt
│   └── manage.py
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── App.jsx
│   ├── package.json
│   └── README.md
└── docs/
    └── arquitectura.md
🎯 Objetivos del Sistema
Para Clientes:

Realizar reservas online
Seleccionar mesa (si >6 personas)
Recibir confirmación de reserva

Para Meseros:

Ver estado de todas las mesas
Gestionar reservas y walk-ins
Cambiar estado de mesas

🚀 Instalación y Uso
Backend
bashcd backend
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
Frontend
bashcd frontend
npm install
npm run dev
📱 Funcionalidades Principales
Backend (API)

POST /api/reserva/ - Crear nueva reserva
GET /api/mesas/ - Listar mesas por estado
POST /api/login/ - Autenticación de mesero
PUT /api/mesa/{id}/estado/ - Cambiar estado de mesa

Frontend Cliente

Formulario de reserva
Selección de mesa (condicional)
Confirmación de reserva

Frontend Mesero

Dashboard de mesas
Gestión de reservas
Control de estados

🔄 Estados de Mesa

Libre: Disponible para reserva
Reservada: Mesa reservada pendiente llegada
Ocupada: Mesa con clientes atendiendo

👥 Equipo de Desarrollo

Desarrollador Full Stack

📝 Notas
Este proyecto está en desarrollo como demostración de habilidades full stack.
