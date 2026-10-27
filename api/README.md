# API · Evaluación RDP

Cloudflare Worker + Neon (Postgres). Endpoints: `GET /evals` y `PUT /evals/:key`.

## Estado
- Base Neon: proyecto **Evaluacion RDP Escorial** (sa-east-1), tabla `rdp_evals` ya creada (`schema.sql`).
- Falta desplegar el Worker y pegar su URL en `../config.js`.

## Despliegue (Cloudflare, conectado a GitHub)
1. Workers & Pages → Create → Import a repository → `Evaluacion-RDP-Escorial`.
2. Root directory: `api`. Nombre del Worker: `evaluacion-rdp-api` (el de `wrangler.toml`).
3. Settings → Variables and secrets → agregar el **secreto** `DATABASE_URL` (connection string de Neon, botón *Connect*).
4. Deploy. Copiar la URL `https://evaluacion-rdp-api.<cuenta>.workers.dev` en `../config.js` → `API_URL`.

El total (sobre 100) se recalcula en el servidor con los pesos de la rúbrica.
