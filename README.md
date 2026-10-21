# Mainline

Gestor de tareas en modo oscuro: saludo según la hora, progreso del día, áreas, agenda, metas semanales y modo enfoque.

Es una sola página estática (`index.html`), sin dependencias ni build.

## Secciones

- **Inicio**: tareas de hoy completadas, pendientes, avance contra la meta semanal, racha, tendencia de 2 semanas, áreas, prioridades y agenda del día.
- **Tareas**: buscador con sugerencias (Vencidas, Prioridad alta, Esta semana…), búsquedas recientes, accesos por área; vista de lista agrupada o tablero.
- **Agenda**: semana navegable con eventos, recordatorios y tareas con hora.
- **Métricas**: tareas cerradas por semana, mes o año contra el periodo anterior, meta semanal, actividad diaria y avance por área.
- **Modo enfoque**: temporizador de 15, 25 o 50 minutos para una tarea.

## Atajos de teclado

| Tecla | Acción |
|---|---|
| `N` | Nueva tarea |
| `/` | Buscar |
| `1`–`4` | Cambiar de sección |
| `Esc` | Cerrar |

## Datos

Los datos se guardan en el `localStorage` del navegador. Usa **Ajustes → Exportar respaldo** para guardar una copia en JSON e **Importar respaldo** para restaurarla en otro navegador o dispositivo.

## Publicar con GitHub Pages

1. Settings → Pages.
2. Source: **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. La app queda en `https://dansan28.github.io/gestor_de_tareas/`.
