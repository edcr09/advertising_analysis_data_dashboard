# Advertising_analysis_data_dashboard
## DA-12 Proyecto de analisis de tendencias de videos de publicidad de una agencia mediante dashboard

Trabajas como analista de vídeos publicitarios en la agencia de publicidad Sterling & Draper. Dedicas mucho tiempo a analizar tendencias de vídeos en YouTube para determinar qué contenido merece atención para la mercadotecnia.

Cada video tiene una categoría específica (entretenimiento, música, noticias y política, etc.), una región y una fecha en que se hace tendencia.

Un video puede estar en la sección de tendencias durante varios días seguidos.

Cada semana, las nuevas empleadas Melanie y Ashok te preguntan esto:

- ¿Qué categorías estaban en las tendencias de la semana pasada?
- ¿Cómo se distribuyeron en diversas regiones?
- ¿Qué categorías fueron particularmente populares en los Estados Unidos?

## Objetivo:

Hacer que el proceso sea automático. Crear un dashboard para el departamento de marketing, que les permita analizar el historial de tendencias de videos en YouTube y responda a sus preguntas de cada semana.

## Consideraciones 

Después de hablar con los administradores de la base de datos, reuniste unos requisitos técnicos:

- Objetivo de negocios: analizar el historial de tendencias de videos en YouTube
- Con qué frecuencia se usará el dashboard: al menos una vez al día
- Usuario objetivo del dashboard: gerentes de planificación de videos publicitarios
- Contenido de los datos del dashboard:
- Tendencias pasadas de videos, ordenadas por día y categoría
- Tendencias de videos, ordenadas por país
- Una tabla de correspondencia entre categorías y países
- Parámetros para agrupar los datos:
- Fecha y hora de tendencia
- Categoría de video
- País

### Descripción de datos:
- Historial de tendencias — valores absolutos ordenados por día (dos gráficos: números absolutos y proporción de porcentaje)
- Eventos, ordenados por país — valores relativos (% de eventos)
- La correspondencia entre las categorías y los países — valores absolutos (una tabla)
- Importancia: todos los gráficos son igualmente importantes

#### Fuentes de datos para el dashboard: tabla de agregación: trending_by_time :
- record_id: la clave primaria
- region: país/región geográfica
- trending_date: fecha y hora
- category_title: categoría del video
- videos_count: número de videos en la sección de tendencias

La tabla está en la base de datos youtube, que se creó especialmente para tus necesidades.
- Intervalo de actualización de los datos: una vez cada 24 horas, a la media noche UTC
- Gráficos, controles de dashboard y su orden:
- [Dashboard_draft](dashboard_draft.jpg)

### Dashboard y presentación
Se crea el dashboard utilizando Tableau, estas son algunas instrucciones de uso del dashboard:
- Filtros, parte superior derecha:
- Para ver un rango de fechas especifico, seleccione las casillas del día o los días que desea visualizar
- Para ver una región especifica, seleccione las casillas de la región o regiones que desea visualizar
- Link: [Dashboard](https://public.tableau.com/app/profile/eduardo.cruz8116/viz/Proyecto_Sprint12/Dashboard1)
- Tambien se prepara una presentación de los resultados para compartir a las encargadas de departamento
- Link: [Presentación](DA-12_Dashboard_presentation.pdf)

