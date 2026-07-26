# Skill: Recordar (Memoria de Primer Plano)

Esta skill permite mantener una memoria de primer plano del proyecto. Lee y escribe el fichero `memoria.md` en la raíz del proyecto.

## Uso

Cuando el usuario invoque esta skill (diciendo "recuerda", "guarda en memoria", "qué recuerdas", "lee memoria", etc.):

1. **Leer siempre** el fichero `memoria.md` de la raíz del proyecto al inicio.
2. **Escribir** en `memoria.md` cuando el usuario pida guardar información.

## Fichero

- **Ruta**: `memoria.md` (raíz del proyecto)
- **Formato**: Markdown libre. Cada entrada debe tener un título o etiqueta descriptiva.

## Formato de entradas

```markdown
## [Fecha] - Título breve
Contenido de lo que se debe recordar.
Puede ser múltiples líneas.
---
```

## Acciones

### Leer memoria
Leer `memoria.md` y mostrar/retornar su contenido al usuario.

### Escribir en memoria
Añadir una nueva entrada al final de `memoria.md` con la información que el usuario quiera recordar. No borrar entradas anteriores a menos que se pida explícitamente.

### Limpiar memoria
Si el usuario lo pide, vaciar o eliminar entradas específicas de `memoria.md`.
