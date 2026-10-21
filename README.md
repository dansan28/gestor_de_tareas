# Mainline

Gestor de tareas minimalista: saludo según la hora, lo importante del día, áreas, tablero y agenda con recordatorios.

Es una sola página estática (`index.html`), sin dependencias ni build.

## Secciones

- **Hoy**: saludo según la hora y el día, tareas vencidas y de hoy, agenda y avance de la semana.
- **Tareas**: búsqueda, filtro por área y agrupación automática (Vencidas, Hoy, Mañana, Esta semana, Más adelante, Sin fecha).
- **Tablero**: Pendiente / En curso / Hecha con arrastrar y soltar.
- **Agenda**: eventos de los próximos 14 días y recordatorios que avisan mientras la página está abierta.
- **Áreas**: Servicio social, Universidad, Proyectos, Personal o las que crees.

## Agregar rápido

```
Estudiar ley de Faraday @vie !alta +universidad
```

Los atajos son opcionales: `@hoy`, `@mañana`, `@vie`, `@25/10` para la fecha; `!alta`, `!media`, `!baja` para la prioridad; `+área` para el área.

## Atajos de teclado

| Tecla | Acción |
|---|---|
| `N` | Nueva tarea |
| `/` | Buscar |
| `1`–`5` | Cambiar de sección |
| `Esc` | Cerrar |

## Datos

Los datos se guardan en el `localStorage` del navegador. Usa **Ajustes → Exportar respaldo** para guardar una copia en JSON e **Importar respaldo** para restaurarla en otro navegador o dispositivo.

## Publicar con GitHub Pages

1. Settings → Pages.
2. Source: **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. La app queda en `https://dansan28.github.io/gestor_de_tareas/`.
