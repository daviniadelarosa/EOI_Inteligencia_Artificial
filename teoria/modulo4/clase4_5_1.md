# 4.5 Chatbots e IA en la relación con el cliente: ética y límites

## 1. El Derecho a la Transparencia
En 2026, la normativa (especialmente en la UE con la AI Act) es muy clara: el cliente tiene derecho a saber que interactúa con una IA.

- Identificación obligatoria: Nunca intentes hacer pasar un bot por un humano. El bot debe presentarse: "Hola, soy Carmen AI, el asistente virtual del restaurante...".

- El peligro del antropomorfismo: Evita que la IA use expresiones que impliquen sentimientos humanos reales ("estoy triste porque no vienes"), ya que puede ser considerado manipulación emocional, especialmente en sectores sensibles o con menores.

- Acceso a un humano: La ética dicta (y pronto la ley lo hará en más regiones) que debe existir siempre un "botón de pánico" para hablar con una persona si la IA no resuelve el problema.

## 2. Privacidad y "Memoria" del Bot 
Volviendo al ejemplo de Casa Carmen y el menú:

Datos Sensibles: Si un cliente escribe por el chat: "Soy alérgico a los frutos secos y tengo una enfermedad crónica", esa información es de alta protección (RGPD).

Límite: El bot no debe almacenar datos de salud de forma permanente sin un consentimiento explícito y reforzado.

Entrenamiento con datos de clientes: Una Pyme no debe usar las conversaciones privadas de sus clientes para "re-entrenar" modelos públicos de IA si no ha anonimizado los datos. Lo que el cliente dice en el chat debe quedarse en el entorno seguro de la empresa.

3. Responsabilidad Legal: El caso del "Bot mentiroso"
Este es un punto crítico: 

**¿Quién es responsable si la IA comete un error?**

- Jurisprudencia actual: Ya hay sentencias (como el famoso caso de Air Canada) donde la empresa fue obligada a cumplir una oferta que el chatbot "se inventó".

- El riesgo en Casa Carmen: Si vuestro bot en Voiceflow dice que el Tataki de Atún cuesta 5€ por un error de alucinación (aunque el PDF diga 13.50€), la Pyme podría verse obligada legalmente a mantener ese precio.

- Límites de seguridad: Hay temas donde la IA no debe entrar. Un bot de restaurante no debe dar consejos médicos sobre alergias si hay riesgo de shock anafiláctico; debe derivar siempre a un humano.

## Ejercicio
**"El dilema del descuento"**

"Vuestro bot de IA detecta que un cliente está muy enfadado porque su reserva falló. De forma autónoma, para calmarlo, el bot le ofrece una cena gratis para 10 personas. El dueño de la Pyme dice que no puede asumir ese coste."

Preguntas: 

1. ¿Debe el restaurante invitar a esas 10 personas legalmente?

2. ¿Cómo configurarían el bot para que tenga un límite ético y financiero (ej. no ofrecer descuentos de más del 10% sin supervisión)?

## 3. Casos Reales de Fallos Éticos y Legales
Tres casos que cambiaron las reglas del juego: 

- El caso Air Canada (El bot que inventó una política): Un chatbot de la aerolínea le prometió a un cliente un descuento por duelo que no existía. La empresa alegó que "el bot era una entidad legal separada" y no era responsable. El juez falló a favor del cliente, obligando a las empresas a ser responsables de lo que sus bots digan.

- El caso DPD (El bot que insultó a la empresa): Un cliente frustrado logró que el chatbot de la empresa de mensajería DPD escribiera poemas sobre lo mala que era la compañía e incluso usara lenguaje soez. Lección ética: Falta de filtros de seguridad (Guardrails).

- El caso Chevrolet (El coche a 1 dólar): Un usuario manipuló el chatbot de un concesionario (usando prompt injection) para que aceptara venderle un Chevy Tahoe por 1 dólar. El bot respondió: "Es un trato, es un acuerdo legalmente vinculante".

## 4. Cuestiones a tener en cuenta

- Sesgos en la Atención: Si el chatbot de "Casa Carmen" prioriza reservas de personas con ciertos apellidos o procedencias (por sesgos en los datos de entrenamiento), la Pyme está cometiendo una falta ética grave. Solución: Auditoría de respuestas.

- El "Derecho a la Intervención Humana": (concepto de Human-in-the-loop). La ética exige que si un cliente está sufriendo (ej. una intoxicación alimentaria y escribe al bot), la IA no intente gestionar eso, sino que lo pase a un humano inmediatamente.

- Transparencia de Datos: ¿Qué hace Voiceflow o la herramienta que usemos con los datos de los clientes?. Las empresas deben configurar sus herramientas para que no usen los datos de los clientes para entrenar modelos globales.

## 5. Sostenibilidad y Ecología: El Coste Oculto de la IA

### A. La Huella Digital de un "Hola"
Debemos concienciarnos de que cada vez que su chatbot responde, se activa una maquinaria física en un centro de datos.

- Consumo energético: Una búsqueda en ChatGPT consume aproximadamente 10 veces más electricidad que una búsqueda en Google. Entrenar un modelo de lenguaje grande puede consumir tanta energía como la que gastan 100 casas españolas en un año.

- Consumo de agua: Los centros de datos necesitan enfriarse. Se estima que por cada conversación de 20-50 preguntas con una IA, se "bebe" medio litro de agua dulce para refrigeración.

- Residuos electrónicos (E-waste): La carrera por la IA obliga a renovar chips (GPUs) cada muy poco tiempo, generando toneladas de residuos difíciles de reciclar.

### B. Estrategias de "IA con Sentido" para Pymes
No se trata de no usar IA, sino de usarla donde realmente aporta valor.

- No matar moscas a cañonazos: No uses el modelo más potente y pesado (como GPT-4o) para tareas simples como corregir una falta de ortografía o saludar. Usa modelos más pequeños y eficientes (Small Language Models o versiones "Mini").

- Filtros de intención: Antes de enviar la pregunta a la IA, usa un código simple (basado en reglas) para ver si la duda es común. Si es una FAQ, responde con texto estático. Si es compleja, entonces llama a la IA.

- Limpieza de Datos: Tener "datos basura" en la base de conocimientos (PDFs duplicados, información obsoleta en el menú de Casa Carmen) hace que la IA trabaje más y consuma más recursos para encontrar la respuesta.

### C. El Dilema del "IA para todo"
A veces, lo más ecológico y ético es el toque humano.

- Saturación digital: Si una Pyme automatiza hasta el último mensaje de felicitación de cumpleaños, pierde la esencia y gasta energía innecesaria en algo que el cliente percibe como artificial.

- Valor añadido: La IA debe liberar tiempo para que el humano haga lo que la IA no puede: empatizar profundamente, resolver conflictos emocionales y cuidar el medio ambiente local.

[Video](https://www.youtube.com/watch?v=RNuDsdLEohk)