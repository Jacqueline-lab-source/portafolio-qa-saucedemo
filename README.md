# 🧪 Proyecto de Pruebas Manuales y Gestión de Defectos - SauceDemo
## 🎯 Alcance y Estrategia de Pruebas (Enfoque ISTQB)

Para garantizar la calidad y estabilidad de la plataforma e-commerce *SauceDemo*, se diseñó y ejecutó una estrategia de pruebas fundamentada en las mejores prácticas de la ingeniería de software y los estándares del **ISTQB**, enfocando el esfuerzo en mitigar los riesgos de negocio en los flujos críticos de la aplicación.

### ⚙️ Tipos de Pruebas Aplicadas
*   **Pruebas Funcionales (Caja Negra):** Evaluadas desde la perspectiva del usuario final para asegurar que las reglas de negocio (inicio de sesión, gestión del carrito y catálogo) se comporten exactamente según lo esperado, sin necesidad de analizar la estructura del código interno.
*   **Pruebas de Regresión:** Ejecutadas sistemáticamente tras la detección e identificación de defectos críticos para verificar que las modificaciones y correcciones en el entorno no hayan afectado negativamente a las funcionalidades que ya operaban correctamente.

### 📋 Técnicas de Diseño de Pruebas Utilizadas
Para optimizar la cobertura de pruebas minimizando el número de escenarios ejecutados, se aplicaron técnicas analíticas basadas en especificaciones:
1.  **Tablas de Decisión:** Utilizadas para mapear y validar de forma exhaustiva las diferentes combinaciones de credenciales en la pantalla de *Login* (usuarios válidos, inválidos, bloqueados y contraseñas incorrectas).
2.  **Análisis de Valores Frontera (BVA) y Transición de Estados:** Empleados en el flujo del carrito de compras y filtros de ordenamiento para comprobar la consistencia de los datos numéricos y los cambios lógicos del estado de la interfaz (ej. la transición del botón de "ADD TO CART" a "REMOVE").

---

## 👤 Información del Analista
* **Nombre:** Jacqueline Luna
* **Rol:** Junior Software Quality Analyst
* **Ubicación:** Asturias, España
* **LinkedIn:** [www.linkedin.com/in/jacqueline-luna-3a63b8232](http://www.linkedin.com/in/jacqueline-luna-3a63b8232)

---

## ## 💻 Sobre la Plataforma de Pruebas
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
