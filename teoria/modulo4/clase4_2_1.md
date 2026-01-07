# 4.2 Chatbots con IA para atención básica al cliente
## 1. Teoría Fundamental: Del Bot de Botones a la IA Conversacional
En 2026, la distinción entre un chatbot tradicional y uno de IA es crítica para una Pyme.

- Chatbots Tradicionales (Basados en reglas): Funcionan como un "elige tu propia aventura". Si el usuario se sale del guion, el bot falla.

- Chatbots con IA (Generativos y RAG): Utilizan modelos de lenguaje (LLM) y una técnica llamada RAG (Generación Aumentada por Recuperación). Esto permite que el bot lea un PDF de la empresa o su página web y responda preguntas específicas basándose solo en esa información, de forma natural y sin programación.

Beneficios clave para la Pyme:

- Disponibilidad 24/7: Atención inmediata sin importar la hora.

- Escalabilidad: Gestiona 100 consultas simultáneas con el mismo coste que una.

- Cualificación de leads: El bot puede preguntar el presupuesto o servicio deseado antes de pasar el contacto a un humano.

- Reducción de carga operativa: Filtra el 80% de las preguntas frecuentes (FAQs).

## 2. Herramienta para la Práctica: 
Voiceflow (Versión Freemium) es una muy buena opción actual. Es visual, potente y tiene un plan gratuito muy generoso para aprendizaje.

- Enlace: [voiceflow](https://www.voiceflow.com/)

- Nivel: No-code (Arrastrar y soltar).

Pasos simples para hacer una práctica: 

- Subir el PDF de un "Menú de Restaurante" o "Tarifas de una Gestoría" en la sección de Knowledge Base.

- Crear un agente nuevo.

- Probar el chat a la derecha y ver cómo la IA responde preguntas complejas usando solo ese documento.

Ejemplo Restaurante : 

- Menú en PDF: [menu](../../assets/menu.pdf)

- Prompt: "Eres un asistente virtual amable del restaurante Casa Carmen. Tu objetivo es ayudar a los clientes con dudas sobre el menú, precios y platos. Si no sabes algo, responde educadamente que no tienes esa información."

### Ejercicio

"El Reto de los 15 minutos": Inventa una Pyme ficticia (ej. una clínica dental). Deben escribir en un bloc de notas 5 servicios y sus precios. Luego, deben configurar un bot en Voiceflow, "alimentarlo" con ese texto y demostrar que el bot puede explicar los precios y dar consejos básicos de salud dental.

[Video_Ejemplo_1](https://www.youtube.com/watch?v=654BzA_c4Zs)

[Video_Ejemplo_2](https://youtu.be/NnQB2583rwQ)

## 3. ¿Cómo funcionan realmente los chatbots de IA?

Los bots actuales ya no funcionan con "palabras clave", sino mediante una arquitectura llamada RAG (Generación Aumentada por Recuperación).

El proceso RAG paso a paso:
1. Indexación (Cerebro previo): El PDF del menú se "trocea" y se convierte en números (vectores) que representan conceptos. Por ejemplo, el sistema entiende que "Pez" y "Bacalao" están relacionados semánticamente.

2. Recuperación (Búsqueda inteligente): Cuando el usuario pregunta "¿Qué tenéis de pescado?", el bot no busca la palabra exacta, sino que "bucea" en el PDF y encuentra el Lomo de bacalao (15.40 €) o el Salmón a la plancha (14.95 €) porque detecta la similitud de conceptos.

3. Aumentación y Generación: El sistema toma esos datos reales y se los pasa al LLM (como GPT-4 o Gemini) con una instrucción: "Usa solo estos datos para responder de forma amable".

Esto evita las "alucinaciones". Si el bot no encuentra "pizza" en el menú, gracias al RAG, responderá que no tienen, en lugar de inventarse un precio o esa es la forma esperada de funcionamiento.

## 4. El Ecosistema de Herramientas 2025-2026 
Además de Voiceflow, existen otras opciones según la necesidad de la Pyme.

En la siguiente tabla podemos ver algunos ejemplos:

| Herramienta | Perfil de uso                 | Ventaja principal                                                             |
|-------------|-------------------------------|-------------------------------------------------------------------------------|
| Botpress    | Desarrolladores / Pymes Tech  | Muy potente para integraciones con bases de datos complejas.                 |
| Tidio       | Ecommerce / Tiendas Online    | Especialista en carritos abandonados y soporte en vivo.                      |
| Darwin AI   | Marketing / Ventas            | Enfocado en "empleados de IA" que reactivan leads por WhatsApp.              |
| Zendesk AI  | Soporte masivo                | Ideal para empresas que ya tienen un gran volumen de tickets.                |

## 5. Evolución: De Chatbots a "Agentes de IA"
Evolución que se ha ido viendo: 

- Multimodalidad: Los bots ya no solo leen texto. Pueden "ver" una foto de una reserva o "escuchar" un audio de un cliente.

- Proactividad: No esperan a que el cliente pregunte. Si detectan que un usuario lleva 2 minutos mirando la sección de "Carnes" del menú de Casa Carmen, pueden intervenir: "¿Te ayudo a elegir entre el Solomillo de ternera (19.95 €) o el Rabo de buey (15.15 €)?".

- Modelo Híbrido: La tendencia clave es la transición fluida. La IA resuelve el 70-80% de dudas, pero detecta frustración y pasa la conversación a un humano al instante.

## Ejercicio propuesto

Revisa el bot que hemos creado y si el usuario habla de "queja/s", el bot de Voiceflow debe mostrar un mensaje diciendo: "Un compañero humano se pondrá en contacto contigo de inmediato".