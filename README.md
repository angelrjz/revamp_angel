# Transformación Física 2026 — V2

PWA privada para registrar ejecución diaria, progreso corporal, entrenamiento de hipertrofia y revisión semanal.

## Publicación

Sube **el contenido de esta carpeta** a la raíz del repositorio conectado a Vercel:

- `index.html`
- `manifest.json`
- `service-worker.js`
- `vercel.json`
- carpeta `icons/`

Vercel publicará automáticamente el nuevo commit.

## Actualización en iPhone

Después del despliegue, abre la URL una vez en Safari con conexión. La V2 usa un caché nuevo y reemplaza la versión anterior. Si la app instalada sigue mostrando la anterior, ciérrala completamente y ábrela de nuevo.

## Datos

Los datos se guardan localmente en el dispositivo. En **SEMANA → Descargar respaldo** se genera un archivo JSON. Ese archivo puede restaurarse mediante **Importar**.

## Funciones V2

- Comidas planeadas, consumidas o modificadas.
- Balance real contra 1,610 kcal y 120–130 g de proteína.
- Cierre diario: energía, hambre, estrés, recuperación y adherencia.
- Peso, cintura, grasa y masa magra.
- Entrenamiento por serie con peso, repeticiones y RIR.
- Lectura semanal.
- Exportación e importación de respaldo.
- Fechas locales, sin depender de UTC.
