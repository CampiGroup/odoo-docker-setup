# Odoo Docker Setup

Entorno completo para ejecutar Odoo 18 junto con PostgreSQL 15 usando Docker y docker-compose.

Este proyecto está diseñado con fines educativos para desplegar un servidor Odoo en una máquina virtual Ubuntu con datos persistentes.

## Servicios
- Odoo 18
- PostgreSQL 15

## Persistencia
Los datos se almacenan en volúmenes del host ubicados en:
- `/srv/odoo-data`
- `/srv/psql-data`

## Acceso
Una vez levantado el entorno, Odoo estará disponible en:
- `http://localhost:8069` (entorno local)
- `https://odoo.campigroup.es` (entorno producción)

# Estructura propuesta para el proyecto
odoo-docker-setup/
├── docker-compose.yml
├── .gitignore
├── .env.example
├── README.md
└── scripts/
    └── init-db.sh (opcional para PostgreSQL)
