# 🎓 EduMed · Metodologías Docentes Innovadoras — CNDFM

> Repositorio interactivo de actividades docentes innovadoras desarrolladas en las Facultades de Medicina españolas, en el marco del **Grupo de Trabajo de Innovación y Metodologías Docentes** de la Conferencia Nacional de Decanos de Facultades de Medicina (CNDFM).

---

## 📖 Descripción

Esta aplicación web recoge y organiza las experiencias de innovación docente compartidas por las Facultades de Medicina de España, agrupadas en **10 metodologías** de referencia. Los datos provienen de una encuesta lanzada a finales de 2025 / principios de 2026 entre los miembros de la CNDFM.

La herramienta permite explorar las actividades de forma visual e interactiva, consultar reflexiones generales, y exportar el catálogo completo en formato Excel.

---

## ✨ Funcionalidades

- **Catálogo de metodologías** — 10 categorías con descripción detallada e información pedagógica expandible.
- **Panel de actividades** — listado de actividades reales por metodología, con descripción, asignatura, formato y docente responsable.
- **Valoración de actividades** — indicación visual (🟢 exitosa / 🔴 con dificultades) basada en la experiencia de los docentes.
- **Enfoques y herramientas** — subpanel con las variantes y enfoques específicos de cada metodología.
- **Reflexiones generales** — principales conclusiones extraídas de la encuesta, organizadas temáticamente.
- **Exportación a Excel** — descarga del catálogo completo en formato `.xlsx`.
- **Carga dinámica desde Google Sheets** — las actividades se actualizan en tiempo real desde una hoja de cálculo pública.

---

## 🗂️ Las 10 Metodologías

| # | Metodología |
|---|-------------|
| 1 | Co-creación curricular con estudiantes |
| 2 | Aprendizaje basado en Design Thinking |
| 3 | Integración de tecnologías digitales, e-learning y simulación |
| 4 | Aprendizaje activo y colaborativo |
| 5 | Enfoque en diversidad, equidad e inclusión |
| 6 | Colaboración internacional e intercultural |
| 7 | Aprendizaje-servicio y compromiso social |
| 8 | Evaluación formativa e innovadora |
| 9 | Desarrollo reflexivo, pensamiento crítico y profesionalismo |
| 10 | Educación interprofesional |

---

## 🚀 Uso

La aplicación es una página HTML estática. Para ejecutarla en local:

```bash
# Clona el repositorio
git clone https://github.com/<tu-usuario>/<tu-repositorio>.git

# Abre el archivo directamente en el navegador
open index.html
```

O bien accede a la versión publicada en **GitHub Pages**:

```
https://<tu-usuario>.github.io/<tu-repositorio>/
```

---

## 📦 Tecnologías utilizadas

| Tecnología | Uso |
|------------|-----|
| HTML5 / CSS3 | Estructura y estilos |
| JavaScript (Vanilla) | Lógica interactiva |
| [Figtree](https://fonts.google.com/specimen/Figtree) (Google Fonts) | Tipografía |
| [SheetJS / xlsx.js](https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js) | Exportación a Excel |
| Google Sheets (CSV público) | Fuente de datos dinámica |
| [corsproxy.io](https://corsproxy.io) | Proxy CORS para carga de datos |

---

## 📊 Fuente de datos

Las actividades se cargan automáticamente desde una **hoja de Google Sheets** publicada en formato CSV:

```
https://docs.google.com/spreadsheets/d/e/[SHEET_ID]/pub?gid=0&single=true&output=csv
```

Si la carga falla (por red o CORS), la aplicación muestra un conjunto de actividades iniciales predefinidas como fallback.

### Columnas esperadas en la hoja de cálculo

| Columna | Descripción |
|---------|-------------|
| `metodologiaId` | ID numérico de la metodología (1–10) |
| `tipo` | Categoría o tipo de actividad |
| `nombre` | Nombre de la actividad |
| `descripcion` | Descripción detallada |
| `asignatura` | Asignatura y titulación |
| `formato` | Formato (PID, experiencia en aula, etc.) |
| `desarrolladaPor` | Universidad de origen |
| `evaluacion` | Tipo de evaluación asociada |
| `presencialidad` | Modalidad (presencial, online, híbrida) |
| `valoracion` | `positiva` o `negativa` |

---

## 🏫 Contexto

Proyecto desarrollado en el marco del **Grupo de Trabajo de Innovación y Metodologías Docentes** de la [CNDFM](https://www.cndfm.org) — Conferencia Nacional de Decanos de Facultades de Medicina Españolas, con sede de referencia en la **Facultad de Medicina de la Universidad de Valladolid (UVa)**.

---

## 📄 Licencia

Este proyecto se distribuye con fines educativos y de difusión académica en el ámbito de las Facultades de Medicina españolas.  
Para reutilización o adaptación, contacta con el Grupo de Trabajo de Innovación de la CNDFM.

---

*Última actualización: 2026 · CNDFM — Innovación y Metodologías Docentes*
