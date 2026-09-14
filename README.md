<div align="center">

  <h1>🎓 Planificador de Calificaciones • GPA Tracker</h1>
  <p><strong>Herramienta web interactiva para calcular, proyectar y gestionar promedios académicos de forma 100% privada y local.</strong></p>

  [![Version](https://img.shields.io/badge/version-1.0.0-7c3aed.svg?style=for-the-badge)](https://github.com/tu-usuario/gpa-tracker)
  [![License](https://img.shields.io/badge/license-MIT-111111.svg?style=for-the-badge)](LICENSE)
  [![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
  [![Client-Side Privacy](https://img.shields.io/badge/privacy-100%25_client_side-2e7d32.svg?style=for-the-badge)](#-privacidad-y-seguridad)

  <br />

  <a href="#-características">Características</a> •
  <a href="#-fórmulas-y-cálculos">Fórmulas</a> •
  <a href="#-privacidad-y-seguridad">Privacidad</a> •
  <a href="#-tecnologías-utilizadas">Tecnologías</a> •
  <a href="#-instalación-y-uso">Instalación</a> •
  <a href="#-licencia">Licencia</a>
</div>

---

## 📌 Descripción

**GPA Tracker** es una aplicación web *zero-backend* pensada para estudiantes universitarios y secundarios que desean planificar su desempeño académico con precisión. 

Permite simular escenarios futuros, calcular qué nota exacta se necesita en el examen final de cada asignatura para alcanzar una meta determinada y visualizar la evolución ponderada del promedio académico (GPA) en escala **0–10**.

---

## ✨ Características Principales

- 📊 **Cálculo de Promedio Ponderado:** Considera el peso en créditos de cada materia para reflejar un GPA real y preciso.
- 🎯 **Calculadora de Nota Requerida:** Determina automáticamente la calificación exacta necesaria en el porcentaje restante de la materia para lograr la nota final deseada.
- 🔮 **Proyección de Metas (GPA Proyectado):** Compara el promedio acumulado actual contra el objetivo deseado en tiempo real.
- 🌙 **Modo Oscuro / Claro:** Interfaz responsiva con diseño *Glassmorphism* optimizado para estudio nocturno y diurno.
- 🛡️ **Privacidad Total (Zero Data Leak):** Los datos procesados se mantienen exclusivamente en la memoria RAM de tu navegador. Sin bases de datos ni registro de usuarios.
- ⚡ **Modo Demostración:** Botón para cargar rápidamente datos de ejemplo y explorar la herramienta al instante.

---

## 🧮 Fórmulas y Cálculos

### 1. Promedio Ponderado Actual ($GPA$)

$$GPA = \frac{\sum (Nota_i \times Créditos_i)}{\sum Créditos_i}$$

### 2. Calificación Necesaria en Examen Final ($N_{necesaria}$)

Dado un porcentaje completado $P_c$ (expresado en decimal $w_c = P_c / 100$) y un porcentaje restante $w_f = 1 - w_c$:

$$N_{necesaria} = \frac{Nota_{deseada} - (Nota_{actual} \times w_c)}{w_f}$$

- Si $N_{necesaria} > 10$, la aplicación alerta que la meta es matemáticamente inalcanzable.
- Si $w_c \ge 100\%$, la materia se marca como **Completada ✓**.

---

## 🔒 Privacidad y Seguridad

> **"Tus datos son tuyos y de nadie más."**

- **Sin Servidor:** La aplicación no realiza peticiones HTTP para almacenar calificaciones.
- **Sin Persistencia no deseada:** Nada se almacena en cookies ni en `localStorage`. Al refrescar o cerrar la pestaña, toda la información se elimina por completo.
- **Transparencia:** Código abierto y auditable en su totalidad.

---

## 🛠️ Tecnologías Utilizadas

- **HTML5 & Vanilla JavaScript (ES6+):** Lógica reactiva en tiempo real sin marcos de trabajo (*frameworks*) pesados.
- **Tailwind CSS (CDN):** Estilizado moderno, adaptable e interactivo (*Glassmorphism effect*).
- **FontAwesome 6:** Iconografía intuitiva y limpia.
- **Google Fonts:** Tipografías *Inter* y *Space Grotesk*.

---

## 🚀 Instalación y Uso Local

No requiere servidores, compilar código ni instalar dependencias de Node.js.

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/tu-usuario/gpa-tracker.git](https://github.com/tu-usuario/gpa-tracker.git)
