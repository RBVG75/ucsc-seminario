# UCSC Seminario de Informática 2026

Presentación animada interactiva para el **Seminario de Robótica & Realidad Virtual XR 2026** de la Universidad Católica de la Santísima Concepción, Sede Chillán.

## Descripción

Video-presentación web autocontenido que reproduce 10 escenas animadas con estética cyberpunk: secuencia de arranque, logo institucional, título del seminario, tarjetas de proyectos, organizador, agenda, información del evento, expositores, llamado a la acción y pantalla de cierre.

## Archivo principal

**`ucsc-seminar.html`** — archivo unico autocontenido (HTML + CSS + JS). Sin dependencias externas. Se abre directamente en cualquier navegador.

## Escenas

| # | Escena | Duracion | Contenido |
|---|--------|----------|-----------|
| 0 | Boot | 6.5s | Secuencia de arranque estilo terminal |
| 1 | UCSC Logo | 5s | Acrónimo UCSC + nombre universidad + sede |
| 2 | Seminario | 5s | Titulo: Robotica & Realidad Virtual XR |
| 3 | Proyectos | 6s | 3 tarjetas: Alpha (IoT), Beta (NLP), Gamma (Blockchain) |
| 4 | Organizador | 7s | Lucía Fuentes, Jefa de Carrera |
| 5 | Agenda | 7s | Horario 09:00 - 13:00 |
| 6 | Info Evento | 5s | Fecha, horario, lugar |
| 7 | Expositores | 5s | 4 speakers |
| 8 | CTA | 5s | Inscripción |
| 9 | Cierre | 5.5s | Logo UCSC + contacto + hashtag |

Duración total: ~63 segundos (loop automático).

## Estética visual

- Fondo oscuro con partículas rojas interconectadas (Canvas)
- Glow rojo (#ff1a1a) sobre fondo negro
- Scanlines y viñeta estilo retro
- Cursor personalizado con efecto glow
- Animaciones CSS: glitch, fade, slide, scale
- Responsive con breakpoint en 768px

## Datos del evento

- **Fecha:** 04 de mayo, 2026
- **Lugar:** Salón Lázaro Cárdenas, Avda. O'Higgins esquina Vegas de Saldías, Chillán
- **Contacto:** lfuentes@ucsc.cl / +56 41 234 5707
- **Hashtag:** #SeminarioInformaticaUCSC

## Como usar

1. Abrir `ucsc-seminar.html` en un navegador
2. La presentación se reproduce automáticamente
3. Controles inferiores derecho: pausar, reiniciar, siguiente escena
4. Barra de progreso en la parte inferior

## Editar contenido

Todo el contenido (nombres, proyectos, horarios, contactos) esta hardcodeado dentro del HTML. Para modificar:

- **Texto:** buscar los elementos HTML dentro de cada `<!-- SCENE -->`
- **Colores:** editar las variables CSS en `:root`
- **Duraciones de escena:** modificar el array `durations` en el `<script>`
- **Animaciones:** ajustar los setTimeout en cada funcion de animacion

## Tecnologias

- HTML5
- CSS3 (custom properties, animations, flexbox)
- JavaScript vanilla (Canvas API, DOM)
- Sin dependencias externas