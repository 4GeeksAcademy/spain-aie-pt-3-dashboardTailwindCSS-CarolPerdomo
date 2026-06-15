# Copilot Instructions

## Objetivo de lo realizado
Se construyo un dashboard operativo responsive llamado **PulseOps Dashboard** enfocado en visualizacion de KPIs, estado de rutas y seguimiento de turno.

## Stack y herramientas usadas
- HTML5 semantico en `index.html`.
- Tailwind CSS v4 por CLI (no CDN) con archivo de entrada `styles.css`.
- Build CSS hacia `dist/output.css`.
- Tipografia principal: Space Grotesk desde Google Fonts.

## Estructura implementada
- Sidebar lateral con:
  - Branding PulseOps.
  - Navegacion interna por anclas: Rendimiento, Drivers y Operacion.
  - Tarjeta de turno actual.
- Header principal con resumen operativo y metadatos (Hub / Fecha).
- Seccion de KPIs clave:
  - Pedidos procesados.
  - SLA expedicion.
  - Coste por envio.
- Seccion de drivers operacionales:
  - Velocidad de picking.
  - Capacidad por franja.
  - Incidencias activas.
- Seccion de detalle operacional:
  - Estado por ruta con vista mobile (cards) y desktop (tabla).
  - Checklist del turno.

## Criterios de UI aplicados
- Paleta personalizada con tokens de color en `@theme` dentro de `styles.css`.
- Diseño con tarjetas, bordes suaves, sombras y jerarquia visual clara.
- Layout responsive con breakpoints de Tailwind para mobile, tablet y desktop.
- Fondo con gradiente suave y bloques de alto contraste para lectura de datos.

## Accesibilidad y semantica
- Uso de etiquetas semanticas: `header`, `nav`, `main`, `section`, `article`, `table`.
- IDs y anclas para navegacion interna.
- Atributos `aria-label` y `aria-labelledby` en zonas de navegacion y datos.
- Metadatos base de SEO: `title`, `description`, `viewport`, `lang`.

## Scripts disponibles
En `package.json`:
- `npm run build:css` compila y minifica CSS a `dist/output.css`.
- `npm run watch:css` recompila automaticamente en modo watch.

## Convenciones para siguientes cambios
- Mantener Tailwind v4 por CLI y seguir compilando a `dist/output.css`.
- Priorizar utilidades Tailwind en HTML y reservar `styles.css` para tema/tokens globales.
- Conservar el enfoque responsive mobile-first.
- Si se agregan nuevas tarjetas o secciones, mantener consistencia visual con radios, sombras y escalas tipograficas actuales.
