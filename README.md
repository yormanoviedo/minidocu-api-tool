# MiniDocuAPITool v1.1.0

**MiniDocuAPITool** es una herramienta ligera, rápida y eficiente diseñada para documentar interfaces de integración (como iFlows de SAP CPI / SAP BTP) de manera sencilla y estructurada. Permite organizar tus APIs por proyectos, gestionar cabeceras HTTP, desglosar sus esquemas de campos de entrada y de respuesta exitosa, reordenar parámetros dinámicamente, duplicar endpoints entre proyectos, visualizar los payloads de petición/respuesta y generar documentación profesional en formato Word.

### 🚀 Características principales

* **Organización por Proyectos:** Agrupa tus iFlows por proyectos para mantener un orden claro.

* **Configuración de Autenticación (Paso 0):** Permite configurar los datos de autenticación OAuth2 Client Credentials (SAP BTP) por proyecto (Token URL, Client ID, Client Secret, Scope y ejemplos de Request/Response).

* **Copiar / Duplicar APIs:** Permite duplicar fácilmente cualquier API documentada asignándola a un nuevo proyecto o al mismo, manteniendo íntegros sus headers, esquemas y payloads.

* **Headers — Cabeceras del Request:** Permite documentar cabeceras requeridas u opcionales (ej: `Accept-Language`, `Content-Type`, `X-Correlation-ID`) con sus valores de ejemplo y descripciones, incluyendo presets de un clic para cabeceras comunes.

* **Schema — Campos del Request:** Desglosa campo a campo los parámetros de entrada del JSON especificando nombre, tipo de dato (Alfanumérico, Numérico, Booleano, Fecha, etc.), obligatoriedad, longitud/formato y descripción.

* **Schema — Campos de la Respuesta (Success):** Especifica la estructura detallada del JSON retornado en respuestas exitosas (HTTP 200/201), indicando nombre del parámetro, tipo, presencia obligatoria u opcional, longitud y descripción.

																																			 

* **Reordenamiento Dinámico de Filas:** Permite reordenar fácilmente la posición de los campos (subir ⬆️ y bajar ⬇️) en las tablas de Headers, Schema de Entrada y Schema de Salida para estructurar la documentación sin necesidad de reescribirla.

* **Gestión Visual Swagger-like:** Interfaz clara e intuitiva con códigos de color según el método HTTP (`GET`, `POST`, `PUT`, `DELETE`).

* **Persistencia Local:** Tus datos se guardan en el navegador (`localStorage`), por lo que no pierdes el trabajo al recargar o cerrar la pestaña.

* **Exportación e Importación de DB:** Exporta tu base de datos a un archivo `.txt` para realizar copias de seguridad o compartirla con tu equipo, e impórtala cuando lo necesites.

* **Documentación Profesional en Word:** Genera documentos técnicos en formato Word (`.doc`) listos para entregar, ya sea de un endpoint individual o de todo un proyecto completo (incluyendo el Paso 0 de Autenticación, las tablas de Headers, Schemas de entrada y salida, y numeración dinámica de secciones).

### 🛠 Instalación

No requiere instalación ni servidores backend. Al ser una herramienta ejecutable en un único archivo HTML:

1. Descarga el archivo `minidocu-api-tool.html`.

2. Ábrelo directamente en tu navegador favorito (*Google Chrome, Microsoft Edge, Firefox, etc.*).

### 💡 Cómo usar

1. **Gestionar Proyectos:** Haz clic en **"Gestionar Proyectos"** para crear un proyecto y, si aplica, configurar los datos de autenticación OAuth2.

2. **Agregar / Editar APIs:** Usa el botón **"+ Agregar API"** para documentar un nuevo endpoint. Puedes añadir cabeceras usando la sección **Headers**, especificar parámetros de entrada en **Schema — Campos del Request** y definir la estructura devuelta en **Schema — Campos de la Respuesta (Success)**.

3. **Duplicar APIs:** Haz clic en el botón **"Copiar"** de cualquier API para crear una réplica rápida en otro proyecto o en el mismo con una nueva denominación.

4. **Reordenar Campos:** Utiliza las flechas de posición en las filas de las tablas para subir o bajar el orden de cualquier header o parámetro.

5. **Copiar Payloads:** En la vista detallada de cada API, utiliza los botones de **"Copiar"** para llevar los JSON directamente a tu portapapeles.

6. **Exportar a Word:** Usa el botón **"Word"** en una API específica o el botón general **"Word (Proyecto)"** para descargar la documentación técnica completa en formato `.doc`.

7. **Backups:** Utiliza **"Exportar DB"** para descargar un respaldo en formato `.txt` antes de limpiar la caché del navegador.

### 🤝 Créditos y Agradecimientos

Este proyecto ha sido ideado y estructurado por **yormanoviedo**.

El desarrollo de esta herramienta ha contado con el apoyo y la colaboración técnica de **Gemini**, asistiendo en la arquitectura, persistencia de datos local, la lógica de generación del esquema dinámico, el reordenamiento de campos, la clonación de APIs entre proyectos, la exportación estructurada a Word y la optimización de la interfaz de usuario.

Hecho con ❤️ para la comunidad de desarrolladores e integradores SAP.
