# Evaluación RDP · Escorial

Sistema de evaluación de Círculos de Calidad / RDP (A3, ciclo PDCA) de Escorial.
Cada evaluador puntúa 10 criterios (escala 1–4 con rúbrica) sobre un total de 100 puntos; la pestaña Resultados arma el ranking, el detalle por criterio y la tabla completa.

| Bloque | Criterios | Puntos |
|---|---|---|
| Plan | P1 Problema, P2 Desglose, P3 Objetivo SMART, P4 Causa raíz, P5 Contramedidas | 10 / 5 / 5 / 20 / 15 |
| Do | P6 Implementación | 20 |
| Check | P7 Resultados | 10 |
| Act | P8 Estandarización | 5 |
| Presentación | Presentación, Reflexión del equipo | 5 / 5 |

Bandas: ≥75 % Excelente · ≥55 % Bueno · ≥35 % En desarrollo · <35 % Insuficiente.

## Uso
- Frontend estático (`index.html` + `config.js`), publicado con GitHub Pages.
- **Modo local** (por defecto): `API_URL` vacío en `config.js`; se guarda en el navegador del dispositivo.
- **Modo compartido**: desplegar el repo [Evaluacion-RDP-API](https://github.com/diegortizdao-collab/Evaluacion-RDP-API) y completar `API_URL`; todos los evaluadores ven el mismo ranking (se refresca cada 15 s).

Una evaluación se identifica por evaluador + círculo: volver a evaluar el mismo círculo con el mismo nombre actualiza la anterior.

---
Desarrollado por Mgter. Diego Ortiz — Líder de Mejora Continua | Consultor ISO
