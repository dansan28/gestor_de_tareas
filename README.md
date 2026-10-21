# Mainline

Gestor de tareas con estética de GitHub: resumen del día con saludo según la hora, repositorios por área, issues filtrables, tablero kanban y agenda con recordatorios.

Es una sola página estática (`index.html`), sin dependencias ni build.

## Funciones

- **Resumen**: saludo según la hora y el día, enfoque de hoy, agenda, recordatorios, hito de la semana y gráfica de actividad.
- **Repositorios**: un repo por área (`servicio-social`, `universidad`, `proyectos`, `personal`) con tareas, tablero y estadísticas propias.
- **Tareas**: lista tipo issues con filtros `is:open`, `is:closed`, `is:doing`, `repo:universidad`, `label:uni`, `prio:alta`, `due:hoy`, `due:vencidas`, `due:semana`, `due:sin`.
- **Tablero**: kanban Por hacer / En progreso / Hecha con arrastrar y soltar.
- **Agenda**: eventos de los próximos 14 días y recordatorios que avisan mientras la página está abierta.

## Captura rápida

```
estudiar faraday +universidad #uni !alta @vie
```

| Token | Significado |
|---|---|
| `+repo` | repositorio |
| `#etiqueta` | etiqueta |
| `!alta` `!media` `!baja` | prioridad |
| `@hoy` `@mañana` `@vie` `@25/10` `@2026-10-25` | fecha límite |

## Atajos

| Tecla | Acción |
|---|---|
| `c` | Nueva tarea |
| `/` | Buscar y filtrar |
| `1`–`5` | Cambiar de sección |
| `Esc` | Cerrar panel |

## Datos

Los datos se guardan en el `localStorage` del navegador. Usa **Ajustes → Exportar respaldo** para guardar una copia en JSON e **Importar respaldo** para restaurarla en otro navegador o dispositivo.

## Publicar con GitHub Pages

1. Settings → Pages.
2. Source: **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. La app queda en `https://dansan28.github.io/gestor_de_tareas/`.
