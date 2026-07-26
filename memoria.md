## 2026-07-27 - MiniDocuAPITool

- **Nombre:** MiniDocuAPITool
- **Ubicación:** /home/yorman/Documentos/opencode_proyectos/
- **Desarrollado por:** yormanoviedo
- **Tipo:** Herramienta web de documentación de APIs
- **Versión:** 1.0.3

### 📋 Descripción
MiniDocuAPITool es una herramienta ligera, rápida y eficiente diseñada para documentar interfaces de manera sencilla. Permite organizar tus APIs por proyectos, visualizar los payloads de petición/respuesta y generar documentación profesional en formato Word.

### ✨ Características principales
- **Organización por Proyectos:** Agrupa tus iFlows por proyectos para mantener el orden
- **Gestión Visual:** Interfaz inspirada en el look-and-feel de Swagger
- **Persistencia Local:** Tus datos se guardan en localStorage, por lo que no pierdes el trabajo al recargar
- **Exportación/Importación:** Exporta tu base de datos a un archivo .txt para realizar backups
- **Documentación Profesional:** Genera documentos en formato Word (.doc) listos para entregar

### 🚀 Instalación
No requiere instalación compleja. Simplemente abre el archivo minidocu-api-tool.html en tu navegador favorito (Chrome, Edge, Firefox).

### 💡 Cómo usar
- **Agregar APIs:** Usa el botón "+ Agregar API" para documentar un nuevo endpoint
- **Gestionar Proyectos:** Crea proyectos para clasificar tus interfaces
- **Exportar:** Usa el botón "Exportar DB" para compartir tu trabajo, o "Word (Proyecto)" para documentación

### 🔧 Tecnología
- **Frontend:** HTML5 + Vanilla JS
- **Estilos:** Tailwind CSS (CDN)
- **Persistencia:** localStorage
- **Exportación:** Generación de Blob para descarga .doc

### 📦 Funcionalidades
- CRUD completo para APIs y proyectos
- Búsqueda de APIs por nombre, ruta o método
- Colapsar/expandir proyectos
- Copiar JSON al portapapeles
- Diseño responsive y colores por método HTTP (GET/POST/PUT/DELETE)
- Validación de datos
- Ejemplos de payloads (Request/Response/Error)

### 🔧 Mejoras Implementadas (2026-07-27)

| # | Mejora | Prioridad |
|---|--------|-----------|
| 1 | **XSS en copy-to-clipboard** - Usando `data-copy-text` con `escapeHtml` en lugar de `onclick` inline | Crítica |
| 2 | **`event` implícito** - Event delegation con `data-*` attributes | Crítica |
| 3 | **Versión inconsistente** - Ahora v1.0.3 en título y badge | Alta |
| 4 | **Accesibilidad ARIA** - `role="dialog"`, `aria-modal`, `aria-label`, `sr-only` | Alta |
| 5 | **Debounce búsqueda** - 250ms delay para evitar rebuild completo del DOM | Media |
| 6 | **Word escaping** - `escapeHtml()` en todos los campos del template Word | Media |
| 7 | **Validación importación** - `validateImportedData()` con campos requeridos | Media |
| 8 | **IIFE + namespace** - Todo envuelto en `(function() { ... })()` con `App.state` | Media |

### 📁 Cambios Técnicos
- Event delegation global en lugar de `onclick` inline
- `data-*` attributes para manejar eventos
- Validación de tipos en importación
- Escape completo en exportación Word
- `<label>` oculto para input de búsqueda

### 🤝 Créditos
Desarrollado con ❤️ por yormanoviedo, con apoyo técnico de Gemini.

---
