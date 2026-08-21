# MiniDocuAPITool v1.0.6

**MiniDocuAPITool** es una herramienta ligera, rápida y eficiente diseñada para documentar interfaces de integración (como iFlows de SAP CPI / SAP BTP) de manera sencilla y estructurada. Permite organizar tus APIs por proyectos, desglosar sus esquemas de campos de entrada, visualizar los payloads de petición/respuesta y generar documentación profesional en formato Word.

### 🚀 Características principales

* **Organización por Proyectos:** Agrupa tus iFlows por proyectos para mantener un orden claro.

* **Configuración de Autenticación (Paso 0):** Permite configurar los datos de autenticación OAuth2 Client Credentials (SAP BTP) por proyecto (Token URL, Client ID, Client Secret, Scope y ejemplos de Request/Response).

* **Schema — Campos del Request:** Desglosa campo a campo los parámetros de entrada del JSON especificando nombre, tipo de dato (Alfanumérico, Numérico, Booleano, Fecha, etc.), obligatoriedad, longitud/formato y descripción.

* **Gestión Visual Swagger-like:** Interfaz clara e intuitiva con códigos de color según el método HTTP (`GET`, `POST`, `PUT`, `DELETE`).

* **Persistencia Local:** Tus datos se guardan en el navegador (`localStorage`), por lo que no pierdes el trabajo al recargar o cerrar la pestaña.

* **Exportación e Importación de DB:** Exporta tu base de datos a un archivo `.txt` para realizar copias de seguridad o compartirla con tu equipo, e impórtala cuando lo necesites.

* **Documentación Profesional en Word:** Genera documentos técnicos en formato Word (`.doc`) listos para entregar, ya sea de un endpoint individual o de todo un proyecto completo (incluyendo el Paso 0 de Autenticación, el desglose del Schema y numeración dinámica de secciones).

### 🛠 Instalación

No requiere instalación ni servidores backend. Al ser una herramienta ejecutable en un único archivo HTML:

1. Descarga el archivo `minidocu-api-tool-v2.html`.

2. Ábrelo directamente en tu navegador favorito (*Google Chrome, Microsoft Edge, Firefox, etc.*).

### 💡 Cómo usar

1. **Gestionar Proyectos:** Haz clic en **"Gestionar Proyectos"** para crear un proyecto y, si aplica, configurar los datos de autenticación OAuth2.

2. **Agregar / Editar APIs:** Usa el botón **"+ Agregar API"** para documentar un nuevo endpoint. Puedes añadir filas dinámicas en la sección **Schema — Campos del Request** para especificar cada parámetro.

3. **Copiar Payloads:** En la vista detallada de cada API, utiliza los botones de **"Copiar"** para llevar los JSON directamente a tu portapapeles.

4. **Exportar a Word:** Usa el botón **"Word"** en una API específica o el botón general **"Word (Proyecto)"** para descargar la documentación técnica completa en formato `.doc`.

5. **Backups:** Utiliza **"Exportar DB"** para descargar un respaldo en formato `.txt` antes de limpiar la caché del navegador.

### 🤝 Créditos y Agradecimientos

Este proyecto ha sido desarrollado por **yormanoviedo**.

El desarrollo de esta herramienta ha contado con el apoyo y la colaboración técnica de **Gemini**, asistiendo en la arquitectura, persistencia de datos local, la lógica de generación del esquema dinámico, la exportación estructurada a Word y la optimización de la interfaz de usuario.

Hecho con ❤️ para la comunidad de desarrolladores e integradores SAP.
