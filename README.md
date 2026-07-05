## Integrantes

- Tere Carmona
- Pablo Quincha
- David Gili

# MercadoLocal — Hito 3 Backend 

API REST modular con Node.js, Express y PostgreSQL. Incluye `pg`, `pg-format`, JWT,
bcrypt, CORS, middlewares y seis pruebas Supertest.

## Puesta en marcha

1. Ejecuta `database/00_crear_base_datos.sql` en la base `postgres`.
2. Conéctate a `mercadolocal_db` y ejecuta `database/schema.sql` y `database/seed.sql`.
3. Ejecuta `npm install`, `npm run dev` y abre `http://localhost:3000/api/health`.
4. Ejecuta `npm test` para comprobar los códigos de estado.

Usuarios demo (contraseña bcrypt):
- `demo@mercadolocal.cl` / `12345678`
- `vendedor@mercadolocal.cl` / `12345678`

## Preparación para producción

`src/config/db.js` acepta tanto variables locales como `DATABASE_URL` y SSL.
`CORS_ORIGINS` acepta varias URLs separadas por coma.
