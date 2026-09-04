# Sistema Unidad Territorial

Plataforma web para la gestión integral de una junta de vecinos, desarrollada como proyecto de título (CAPSTONE) de Ingeniería en Informática, Duoc UC — Sede San Joaquín.

## Descripción

El **Sistema Unidad Territorial** centraliza la gestión administrativa y la participación de los vecinos de una unidad territorial, reemplazando procesos hoy realizados de forma manual (inscripciones, certificados, postulación de proyectos y comunicación con la comunidad).

El sistema está compuesto por dos módulos conectados a una misma base de datos:

- **Módulo interno** — para el directorio de la junta: administración de inscripciones, emisión de certificados, revisión de postulaciones de proyectos, envío de notificaciones y publicación de noticias.
- **Módulo público** — para los vecinos: inscripción, solicitud de certificados, postulación a proyectos, reserva de espacios comunes y recepción de avisos.

## Funcionalidades principales

- [ ] Autenticación y roles de usuario (directorio / vecino)
- [ ] Inscripción y gestión de vecinos
- [ ] Emisión y solicitud de certificados de residencia
- [ ] Postulación y revisión de proyectos vecinales
- [ ] Reserva de espacios comunes
- [ ] Publicación de noticias y avisos
- [ ] Notificaciones vía email y/o WhatsApp
- [ ] Diseño responsivo (acceso desde celular y computador)

## 🛠️ Tecnologías

| Capa | Tecnología |
|---|---|
| Backend | PHP + Laravel |
| Base de datos | MySQL |
| Frontend | Bootstrap |
| Control de versiones | Git / GitHub |

## Instalación

```bash
# Clonar el repositorio
git clone https://github.com/usuario/sistema-unidad-territorial.git
cd sistema-unidad-territorial

# Instalar dependencias PHP
composer install

# Configurar variables de entorno
cp .env.example .env
php artisan key:generate

# Configurar la base de datos en .env (DB_DATABASE, DB_USERNAME, DB_PASSWORD)

# Ejecutar migraciones
php artisan migrate

# (Opcional) Poblar con datos de prueba
php artisan db:seed

# Levantar el servidor local
php artisan serve
```

El sistema quedará disponible en `http://localhost:8000`.

## Estructura del proyecto

```
sistema-unidad-territorial/
├── app/            # Lógica de negocio (modelos, controladores)
├── database/       # Migraciones y seeders
├── public/         # Punto de entrada y assets públicos
├── resources/       # Vistas (Blade), CSS, JS
├── routes/         # Definición de rutas web
└── tests/          # Pruebas funcionales
```

## Metodología

Proyecto desarrollado de forma **individual** bajo metodología **Iterativo-Incremental**, en cinco etapas: levantamiento de requerimientos, diseño (arquitectura, BD y UI/UX), desarrollo iterativo por módulos, pruebas y certificación, y cierre con documentación.

## Evidencias del proyecto

- Documento de planificación y diseño (arquitectura, GUI, BD)
- Documentos de control y pruebas
- Documentos de cierre del proyecto
- Sistema web funcional (este repositorio)

## Autora

**Francisca Baeza Madariaga**
Ingeniería en Informática — Duoc UC, Sede San Joaquín
Asignatura CAPSTONE, Sección 300D

## Licencia

Proyecto académico desarrollado con fines educativos.
