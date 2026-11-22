# PhotoSpot PWA v0.1

Prototipo de uso personal para iPhone, desarrollado con HTML, CSS y JavaScript desde Windows.

## Cómo probar en iPhone

1. Extrae el ZIP.
2. Publica la carpeta en un alojamiento estático HTTPS (por ejemplo, GitHub Pages). No basta con abrir index.html como archivo local: la geolocalización requiere un contexto seguro.
3. Abre la URL HTTPS en Safari del iPhone y concede permiso de ubicación.
4. Usa Compartir > Añadir a pantalla de inicio.
5. Con el vehículo estacionado, pulsa Iniciar recorrido GPS. Espera suficientes muestras, prueba Marcar aquí y Marcar atrás y abre una ruta.

## Límites

- No implementa reconocimiento de voz ni Siri. No debe usarse pulsando botones mientras se conduce.
- iOS puede suspender el seguimiento GPS, incluso con la pantalla encendida.
- Marcar atrás elige una muestra GPS anterior a la hora objetivo; no garantiza precisión temporal ni espacial.
- Los puntos se almacenan en localStorage del navegador; exporta copias JSON periódicas. Limpiar los datos de Safari puede eliminarlos.
- Para privacidad, elige cuidadosamente dónde alojar el sitio; las coordenadas guardadas no se suben por este código, pero el proveedor de alojamiento puede registrar visitas.
- Google Maps se abre mediante Maps URLs, sin API de pago.
