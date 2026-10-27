# API · Evaluación RDP

Cloudflare Worker + Neon (Postgres). Dos endpoints: `GET /evals` y `PUT /evals/:key`.

1. Crear el proyecto en Neon y ejecutar `schema.sql`.
2. `cd api && npm install`
3. `npx wrangler secret put DATABASE_URL` (connection string de Neon)
4. Ajustar `ALLOWED_ORIGIN` en `wrangler.toml` y `npx wrangler deploy`
5. Pegar la URL del Worker en `../config.js` (`API_URL`) y hacer commit.

El total (sobre 100) se recalcula en el servidor con los pesos de la rúbrica.
