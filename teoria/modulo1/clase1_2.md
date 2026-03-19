# 1.2 Modelos de lenguaje: ChatGPT, Perplexity, Gemini, Copilot y Claude

## Qué son los modelos de lenguaje

Los modelos de lenguaje (LLMs, por sus siglas en inglés) son sistemas de IA entrenados con enormes volúmenes de texto para **comprender y generar lenguaje de forma coherente**.

> **Analogía sencilla:** Funcionan como un autocompletador muy sofisticado. Han leído más texto del que cualquier persona podría leer en mil vidas, y usan ese conocimiento para responder preguntas, redactar contenido, resumir documentos o razonar sobre un problema.

### Cómo funcionan (lo esencial)

1. Se entrenan con grandes volúmenes de texto (libros, artículos, webs).
2. Dado un mensaje o instrucción (*prompt*), predicen la respuesta más útil.
3. Se refinan con retroalimentación humana para mejorar calidad y seguridad.

---

## Capacidades principales

- **Generación de texto:** emails, informes, artículos, guiones, propuestas comerciales.
- **Transformación:** traducción, simplificación, reescritura con distinto tono o formato.
- **Análisis:** extracción de ideas clave, categorización, detección de sentimientos en reseñas.
- **Creatividad:** lluvia de ideas, naming, slogans, storytelling.
- **Soporte técnico:** explicación de conceptos, generación de código, documentación.

---

## Limitaciones y riesgos

- **Alucinaciones:** pueden generar respuestas plausibles pero incorrectas. Verificar siempre datos concretos.
- **Sesgos:** reproducen prejuicios presentes en los datos de entrenamiento.
- **Privacidad:** riesgo si se introducen datos sensibles de clientes, empleados o financieros.
- **Desactualización:** algunos modelos no tienen acceso a información en tiempo real.
- **Dependencia:** pueden fomentar exceso de confianza si no se validan los resultados.

---

## Herramientas destacadas

### ChatGPT (OpenAI)
- **Fortalezas:** generación de contenido creativo y estructurado, razonamiento general, amplio ecosistema de integraciones y plugins.
- **Usos en PYMEs:** redacción de emails y propuestas, creación de manuales, generación de posts para redes sociales, asistente de ventas.
- **Limitaciones:** puede inventar datos con confianza; requiere supervisión humana.

### Perplexity
- **Fortalezas:** respuestas con citas y enlaces a fuentes verificables, orientado a búsqueda e investigación.
- **Usos en PYMEs:** investigación de mercado, análisis de competencia, recopilación de información con fuentes contrastadas.
- **Limitaciones:** depende de la calidad de las fuentes indexadas; menos potente para generación creativa.

### Gemini (Google)
- **Fortalezas:** integración nativa con el ecosistema Google (Docs, Sheets, Gmail, Meet), capacidades multimodales (texto, imagen, audio).
- **Usos en PYMEs:** documentación en Google Docs, análisis de hojas de cálculo, generación de presentaciones en Google Slides.
- **Limitaciones:** privacidad sujeta a las políticas de Google; algunos planes requieren Google Workspace de pago.

### Microsoft Copilot
- **Fortalezas:** integración nativa con Microsoft 365 (Word, Excel, Outlook, Teams, PowerPoint). Si tu empresa ya usa el paquete de Microsoft, es la opción de menor fricción para empezar.
- **Usos en PYMEs:** redactar y resumir emails en Outlook, analizar datos en Excel, generar presentaciones en PowerPoint, tomar notas automáticas en reuniones de Teams.
- **Limitaciones:** requiere licencia Microsoft 365 Business; el Copilot avanzado tiene coste adicional.

### Claude (Anthropic)
- **Fortalezas:** muy fiable en análisis de documentos largos, redacción detallada y razonamiento cuidadoso. Destaca por sus buenas prácticas de seguridad y privacidad.
- **Usos en PYMEs:** revisión y resumen de contratos largos, análisis de informes, redacción de documentación técnica, soporte en decisiones complejas.
- **Limitaciones:** ecosistema de integraciones más limitado que ChatGPT o Copilot.

---

## Comparativa rápida: precios y acceso

| Herramienta | Plan gratuito | Plan de pago (aprox.) | Mejor integración |
|---|---|---|---|
| **ChatGPT** | Sí (GPT-4o limitado) | ~20 €/mes/usuario | API, plugins, web |
| **Perplexity** | Sí | ~20 €/mes/usuario | Búsqueda web con fuentes |
| **Gemini** | Sí | Incluido en Google Workspace | Google Docs, Sheets, Gmail |
| **Microsoft Copilot** | Sí (básico) | Incluido en M365 Business / addon | Word, Excel, Teams, Outlook |
| **Claude** | Sí | ~20 €/mes/usuario | Documentos largos, análisis |

> **Recomendación práctica:** empieza con el plan gratuito de la herramienta que mejor encaje con las aplicaciones que ya usas. Escala solo cuando identifiques un caso de uso con retorno claro.

---

## ¿Cuál uso según mi situación?

| Si en tu empresa ya usáis… | Empieza por… |
|---|---|
| Microsoft 365 (Word, Outlook, Teams) | **Microsoft Copilot** |
| Google Workspace (Gmail, Docs, Sheets) | **Gemini** |
| Necesitas buscar información con fuentes | **Perplexity** |
| Contenido creativo y marketing | **ChatGPT** |
| Análisis de documentos largos o contratos | **Claude** |
| Quieres probar sin comprometerte con ninguno | **ChatGPT** (la más extendida) |

---

## Prompt Engineering: cómo hablar con la IA

El **prompt** es la instrucción que damos al modelo. La calidad del resultado depende en gran medida de cómo lo formulamos.

### Principios básicos

1. **Claridad:** especificar contexto, rol, audiencia y objetivo.
2. **Estructura:** dividir en pasos o requisitos claros.
3. **Formato:** indicar cómo queremos la salida (tabla, lista, email, bullet points).
4. **Iteración:** refinar el prompt según el resultado obtenido.
5. **Verificación:** comprobar siempre exactitud y relevancia antes de usar.

### Plantilla de prompt eficaz

```
Actúa como [rol].
Para [audiencia], redacta [tipo de contenido] con tono [tono].
Usa estos datos o contexto: [datos relevantes].
Entrega el resultado en [formato], con [criterios de calidad o longitud].
```

### Ejemplo aplicado

> Actúa como especialista en marketing digital. Redacta un email de 150 palabras para PYMEs en Madrid, presentando un nuevo servicio de consultoría en IA. Incluye 3 beneficios claros, tono profesional y una llamada a la acción.

---

## Buenas prácticas de uso en PYMEs

- **No introducir datos sensibles:** proteger información de clientes, empleados y finanzas.
- **Revisión humana obligatoria:** validar siempre antes de enviar o publicar.
- **Transparencia:** declarar el uso de IA en contenidos públicos cuando sea relevante.
- **Documentación interna:** crear guías de prompts y políticas de uso para el equipo.
- **Medición de impacto:** evaluar tiempo ahorrado, calidad del resultado y satisfacción del equipo.

---

## Ejemplos de prompts por sector

### Comercio minorista

**Email de promoción:**
> Actúa como especialista en marketing para comercio minorista.
> Redacta un email de 150 palabras dirigido a clientes habituales de una tienda de ropa en Madrid.
> Incluye una promoción de temporada (20% descuento), 3 beneficios del producto y una llamada a la acción clara.
> Usa un tono cercano y profesional.

**Publicación en redes sociales:**
> Genera un post para Instagram de una tienda de alimentación local.
> El objetivo es anunciar la llegada de productos ecológicos.
> Usa un tono fresco y amigable, incluye 3 hashtags relevantes y una invitación a visitar la tienda.

---

### Servicios profesionales

**Documento resumen:**
> Actúa como consultor en transformación digital.
> Resume en 300 palabras las principales ventajas de implementar IA en una PYME de servicios.
> Organiza el texto en 3 apartados: eficiencia, innovación y competitividad.
> Usa un tono formal y orientado a directivos.

**Guion de llamada comercial:**
> Redacta un guion de 2 minutos para una llamada telefónica de una asesoría fiscal a potenciales clientes.
> Incluye: presentación breve, 3 beneficios del servicio, ejemplo de ahorro y cierre con invitación a reunión.
> Usa un tono profesional y persuasivo.

---

### Industria ligera

**Informe técnico:**
> Actúa como ingeniero de procesos.
> Redacta un informe de 400 palabras sobre cómo la IA puede optimizar la gestión de inventario en una empresa de fabricación de muebles.
> Incluye ejemplos de predicción de demanda, reducción de costes y mejora en tiempos de entrega.
> Usa un tono técnico y estructurado.

**Ideas de innovación:**
> Genera 5 ideas innovadoras para aplicar IA en un taller mecánico de tamaño medio.
> Clasifica las ideas en: atención al cliente, gestión de repuestos, mantenimiento predictivo, formación de empleados y marketing.
> Usa un formato de lista con explicación breve de cada idea.

---

## Casos de uso de IA por sector en PYMEs

| Sector | Casos de uso principales | Ejemplos prácticos |
|---|---|---|
| **Comercio minorista** | Marketing y promociones · Atención al cliente · Gestión de inventario | Emails de ofertas personalizadas · Chatbots para consultas · Predicción de demanda |
| **Servicios profesionales** | Documentación y reporting · Captación de clientes · Formación interna | Resúmenes de informes · Guiones de llamadas comerciales · Microcursos generados con IA |
| **Industria ligera** | Optimización de procesos · Mantenimiento predictivo · Innovación de producto | Análisis de inventario · Alertas de fallos en maquinaria · Generación de ideas de mejora |

---

## Conexión con el trabajo final

Los aprendizajes de este módulo se integran en tres entregables del proyecto:

- **Guía de prompts corporativos:** estándar interno para tareas clave de la empresa.
- **Evaluación comparativa de herramientas:** decisión razonada sobre qué modelo usar en cada área.
- **Política de uso responsable:** marco de gobernanza para la adopción de IA.

---

## Ejercicios

### Ejercicio 1.2 A — Guía de prompts corporativos

**Objetivo:** Crear una guía interna de prompts reutilizables para 3 áreas (ej.: ventas, marketing, atención al cliente).

**Pasos:**

1. Definir 3 tareas clave por área. Ejemplo:
   - Ventas: *"redactar email de propuesta comercial"*
   - Marketing: *"generar post de LinkedIn sobre novedad de producto"*
   - Atención: *"resumir feedback de clientes de la semana"*

2. Diseñar prompts base con variables intercambiables:
   > *"Actúa como [rol]. Para [audiencia], redacta [tipo de contenido] con tono [tono], usando estos datos: [datos]. Entrega en [formato], con [criterios de calidad]."*

3. Probar cada prompt en al menos dos herramientas (ChatGPT, Gemini, Copilot…). Comparar resultados y refinar.

4. Documentar versiones: prompt v1, v2 y qué cambió en cada iteración.

**Entregable para el trabajo final:** "Guía de prompts corporativos v1" con 9 prompts (3 áreas × 3 tareas) y notas de uso.

---

### Ejercicio 1.2 B — Política interna de uso de IA

**Objetivo:** Esbozar una política breve (1–2 páginas) para el uso responsable de IA en la empresa.

**Contenido mínimo:**

- **Privacidad y datos:** qué datos se permiten usar, cuándo anonimizar, qué está prohibido subir.
- **Revisión humana:** cuándo es obligatoria antes de usar el resultado externamente.
- **Transparencia:** cuándo declarar que un contenido ha sido generado con IA.
- **Calidad y control:** checklist de verificación; cómo citar fuentes y evidencias.
- **Cumplimiento legal:** propiedad intelectual, derechos de autor, confidencialidad y marca.

**Entregable para el trabajo final:** "Política interna de IA v1" revisada y aprobada por dirección.
