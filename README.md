# 🧪 Proyecto de Pruebas Manuales y Gestión de Defectos - SauceDemo

## 👤 Información del Analista
* **Nombre:** Jacqueline Luna
* **Rol:** Junior Software Quality Analyst
* **Ubicación:** Asturias, España
* **LinkedIn:** [www.linkedin.com/in/jacqueline-luna-3a63b8232](http://www.linkedin.com/in/jacqueline-luna-3a63b8232)

---

## 🎯 Alcance del Proyecto
Este proyecto contiene el ciclo completo de diseño de pruebas estructuradas, ejecución funcional E2E y reporte técnico de defectos críticos para la plataforma e-commerce **SauceDemo**. Las pruebas se enfocaron en validar los flujos principales del usuario estándar (`standard_user`), así como el control de accesos y la integridad de la interfaz web.

---

## 📁 Estructura del Repositorio
* **`1-docs/`**: Contiene la suite de Casos de Prueba (`casos_de_prueba.txt`) estructurados con precondiciones, pasos y resultados esperados, además del reporte detallado del defecto crítico detectado.
* **`2-evidence/`**: Evidencias visuales de la ejecución de los casos de prueba exitosos (`CP_01` a `CP_04`) y una sección dedicada con capturas resaltadas y video técnico (`.mp4`) para la réplica del Bug.
* **`3-logs/`**: Volcado de errores real extraído directamente de la consola del navegador (`Browser Console Logs`) que respalda la causa raíz del defecto crítico.

---

## 🛠️ Habilidades Técnicas Aplicadas
* **Estrategia de Testing:** Pruebas Estructuradas (Test Cases), Pruebas Funcionales End-to-End (E2E), Regresión y Testing Exploratorio.
* **Gestión de Defectos:** Reporte técnico de incidencias con análisis de causa raíz.
* **Herramientas de Evidencia:** Capturas técnicas resaltadas, grabación de pantalla de réplica y extracción de Console Logs del navegador.

---

## 🐛 Resumen del Defecto Crítico Detectado (BUG-001)
* **Incidencia:** El botón "ADD TO CART" del producto *Sauce Labs Fleece Jacket* cambia visualmente a "REMOVE" al hacer clic, pero no añade el artículo al carrito (el contador permanece en 0) ni actualiza el estado interno de la sesión.
* **Causa Raíz:** Error interno de red (Error 404 / 500 simulado en la API del servidor al procesar el ID específico del producto), validado en los logs adjuntos.
https://github.com/user-attachments/assets/4464374d-68bd-428f-9002-a77387a94f65
