# 🧠 Filosofía 6.º Año — Apps Educativas Gamificadas

**Prof. Julio Alberto Lazarte · Escuela Amado Juri · Tucumán, Argentina**

Apps interactivas de filosofía para alumnos de 6.º año de secundaria, desplegadas en GitHub Pages como archivos HTML únicos autocontenidos. Estética cyberpunk/gamer oscura. Sin dependencias externas en tiempo de ejecución.

---

## 🗂️ Estructura del proyecto

```
juliolaz.github.io/
│
├── UNIDAD 1 — Introducción a la Filosofía
│   ├── Tema 1 — Contexto Histórico
│   │   ├── index_timeline.html        → Línea del Tiempo interactiva
│   │   └── chronos_timeline.html      → Quiz Chronos · Tema 1
│   │
│   ├── Tema 2 — Del Arché a la Metafísica
│   │   ├── index.html                 → App de contenido
│   │   └── chronos_arche_metafisica.html → Quiz Chronos · Tema 2
│   │
│   ├── Tema 3 — ¿Qué es Filosofar?
│   │   ├── filo_que_es_filosofar.html → App de contenido     ✅ NUEVO
│   │   └── chronos_filosofar.html     → Quiz Chronos · Tema 3 🔜
│   │
│   └── Tema 4 — Lógica Informal y Falacias
│       ├── filo_falacias.html         → App de contenido     🔜
│       └── chronos_falacias.html      → Quiz Chronos · Tema 4 🔜
│
├── UNIDAD 2 — Gnoseología           🔜 planificada
├── UNIDAD 3 — Lógica y Argumentación 🔜 planificada
└── UNIDAD 4 — Pensamiento Crítico    🔜 planificada
```

---

## ✅ Apps disponibles

| Archivo | Tema | Tipo | Estado |
|---|---|---|---|
| `index_timeline.html` | U1·T1 — Contexto histórico | Contenido | ✅ Activa |
| `chronos_timeline.html` | U1·T1 — Contexto histórico | Quiz | ✅ Activa |
| `index.html` | U1·T2 — Arché y Metafísica | Contenido | ✅ Activa |
| `chronos_arche_metafisica.html` | U1·T2 — Arché y Metafísica | Quiz | ✅ Activa |
| `filo_que_es_filosofar.html` | U1·T3 — ¿Qué es Filosofar? | Contenido | ✅ Activa |
| `chronos_filosofar.html` | U1·T3 — ¿Qué es Filosofar? | Quiz | 🔜 En desarrollo |
| `filo_falacias.html` | U1·T4 — Falacias | Contenido | 🔜 En desarrollo |
| `chronos_falacias.html` | U1·T4 — Falacias | Quiz | 🔜 En desarrollo |

---

## 🎮 Características técnicas

- **HTML único autocontenido** — cada app es un solo archivo `.html` sin dependencias externas
- **Offline-capable** — funciona sin conexión una vez cacheada (solo fuentes requieren internet)
- **Mobile-first** — optimizado para celulares de alumnos
- **Estética cyberpunk/gamer** — fondo oscuro `#04040e`, fuentes Cinzel + Rajdhani + Crimson Pro
- **Partículas animadas** con Canvas API
- **Scroll reveal** con IntersectionObserver
- **Nav sticky** con barra de progreso por capítulo
- **Cards acordeón** expandibles por sección

---

## 📊 Sistema de Quiz Chronos

Los quizzes envían resultados automáticamente a **Google Sheets + Telegram** vía Google Apps Script.

### Campos enviados por cada intento

| Campo | Descripción |
|---|---|
| `nombre` | Nombre del alumno |
| `apellido` | Apellido |
| `curso` | Curso seleccionado |
| `nivel` | Dificultad elegida (Aprendiz / Filósofo / Maestro) |
| `score` | Puntos obtenidos |
| `pct_correctas` | % de respuestas correctas |
| `pct_aprobacion` | Umbral de aprobación del nivel |
| `aprobado` | true / false |
| `correctas` | Cantidad de respuestas correctas |
| `incorrectas` | Cantidad de respuestas incorrectas |
| `tiempo_agotado` | Preguntas perdidas por tiempo |
| `racha_max` | Racha máxima de respuestas correctas |
| `fecha` | Timestamp del intento |
| `unidad` | Número de unidad |
| `tema` | Tema dentro de la unidad |

### GAS Endpoint

```
https://script.google.com/macros/s/AKfycbxHuPBB9MW0pMXNh-i8m48T3DFULKKAMxdu6lzkYRPO20JSPp4OCInpMrKDWrzDhHnN/exec
```

### Versión del GAS receptor

`gas_chronos_quiz_v3.js` — maneja todas las unidades y temas mediante el campo `unidad`+`tema`.

---

## 🎓 Enfoque pedagógico

- Alumnos vulnerables de secundaria con baja confianza académica
- Filosofía accesible y motivadora, sin jerga abstracta innecesaria
- Ejemplos 100% argentinos y cotidianos (redes sociales, política, fútbol, economía)
- Gamificación: niveles de dificultad, rachas, timer, barra de aprobación
- Lógica **informal** — el alumno detecta errores en frases reales, no fórmulas simbólicas
- Falacias priorizadas por frecuencia en redes y debates políticos argentinos

---

## 🗺️ Secuencia didáctica completa

```
Unidad 1 · Introducción a la Filosofía
  ├── T1 · Contexto histórico         ✅
  ├── T2 · Del Arché a la Metafísica  ✅
  ├── T3 · ¿Qué es Filosofar?         ✅ contenido  /  🔜 quiz
  └── T4 · Lógica Informal            🔜 contenido  /  🔜 quiz

Unidad 2 · Gnoseología básica         🔜
Unidad 3 · Lógica y argumentación     🔜
Unidad 4 · Pensamiento crítico        🔜
```

---

## 👤 Autor

**Julio Alberto Lazarte**
Profesor de Filosofía · 6.º Año Secundaria
Escuela Amado Juri · Tucumán · Argentina
GitHub: [@JulioLaz](https://github.com/JulioLaz)
Sitio: [juliolaz.github.io](https://juliolaz.github.io)

---

*© 2026 — Uso educativo exclusivo*