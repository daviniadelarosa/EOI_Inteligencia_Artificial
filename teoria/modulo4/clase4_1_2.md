# Ejemplos prácticos

## 1. Ejemplos de Aplicación Estratégica
En lugar de solo saber si un comentario es "positivo", estas aplicaciones buscan extraer valor de negocio:

### A. Monitorización de Lanzamientos (Beta Testing)
Si una pyme lanza un nuevo producto (ej. una crema orgánica), el análisis de sentimiento no solo mide la aceptación, sino que segmenta por atributos.

Ejemplo: El modelo detecta sentimiento positivo en "aroma" y "textura", pero neutro/negativo en "diseño del envase".

Acción de Marketing: Pivotar la inversión publicitaria hacia los beneficios sensoriales y rediseñar el packaging en el siguiente lote.

### B. Análisis de la Competencia (Social Listening)
Analizar las reseñas de Google Maps o comentarios de Instagram de la competencia directa.

Ejemplo: Detectar que el sentimiento de los clientes de la competencia cae drásticamente los viernes por la tarde debido al tiempo de espera.

Acción de Marketing: Lanzar campañas de "Atención rápida sin esperas" segmentadas para los viernes.

### C. Clasificación de Tickets de Soporte
Priorizar la atención al cliente no por orden de llegada, sino por carga emocional.

Ejemplo: Un script de Python clasifica los correos. Un mensaje con sentimiento "Muy Negativo" y palabras clave como "devolución" o "fraude" sube al inicio de la cola.

## 2. Ejercicios Prácticos para Pymes que se pueden hacer para analizar sentimiento en Redes
Estos ejemplos están pensados para ser ejecutados con herramientas accesibles, como en código.

### Ejercicio 1: Matriz de Sentimiento vs. Volumen (Priorización)
- Objetivo: Identificar qué problemas reales afectan más a la marca.

- Exporta los últimos 100 comentarios de tus redes sociales a un CSV.

- Clasifica cada comentario en una escala del -1 (muy negativo) al 1 (muy positivo).

- Categoriza por tema: "Precio", "Calidad", "Envío", "Atención".

- Tarea: Calcula el sentimiento promedio por categoría. Si "Envío" tiene un volumen alto de comentarios pero un sentimiento de -0.8, tienes una crisis logística, no de marketing, usando una IA como ChatGPT o Perplexity.


### Ejercicio 2: Refactorización de Copywriting basado en Sentimiento
- Objetivo: Adaptar el lenguaje de la marca al lenguaje real del cliente.

- Toma las 20 reseñas más positivas de tu negocio.

- Extrae los adjetivos y verbos con mayor polaridad positiva (ej. "increíblemente fácil", "me salvó el día").

- Tarea: Redacta un anuncio de Facebook Ads utilizando exclusivamente esas palabras y estructuras gramaticales detectadas. Compara el CTR (Click-Through Rate) con un anuncio escrito de forma genérica.

### Ejercicio 3: Detección de Ironía y Sarcasmo (Avanzado)
- Objetivo: Evitar falsos positivos en los reportes mensuales.

- Analiza este corpus de frases de clientes:

"Gracias por tardar tres semanas en contestar, sois unos cracks."

"Me encanta que el paquete llegara abierto, gran servicio."

- Tarea: Si usas una herramienta básica, estas frases darán "Positivo" por palabras como "gracias", "cracks" o "me encanta". El ejercicio consiste en ajustar el modelo (o usar prompts de ChatGPT o Perplexity) para que detecte la discrepancia entre el verbo positivo y el contexto negativo.



