# 1.2 Modelos de lenguaje: ChatGPT, Perplexity, Gemini

## Qué son los modelos de lenguaje
Los modelos de lenguaje (LLMs, por sus siglas en inglés) son sistemas de IA entrenados con grandes volúmenes de texto para **predecir y generar palabras** de manera coherente. Funcionan como "autocompletadores inteligentes" que, gracias a su escala y entrenamiento, pueden:
- Comprender instrucciones en lenguaje natural.
- Generar texto en múltiples estilos y formatos.
- Resumir, traducir y transformar información.
- Razonar y dar soporte en tareas complejas.

### Cómo funcionan
- **Entrenamiento:** se alimentan con corpus masivos de datos (libros, artículos, webs).
- **Arquitectura:** suelen basarse en *transformers*, capaces de manejar relaciones entre palabras en contexto.
- **Inferencia:** dado un prompt, predicen la siguiente palabra más probable, ajustando el resultado a la instrucción.
- **Fine-tuning y RLHF:** se afinan con retroalimentación humana para mejorar calidad y seguridad.

---

## Capacidades principales
- **Generación de texto:** emails, informes, artículos, guiones.
- **Transformación:** traducción, simplificación, reescritura con distinto tono.
- **Análisis:** extracción de ideas clave, categorización, detección de sentimientos.
- **Creatividad:** lluvia de ideas, storytelling, slogans.
- **Soporte técnico:** explicación de conceptos, generación de código, documentación.

---

## Limitaciones y riesgos
- **Alucinaciones:** respuestas plausibles pero incorrectas.
- **Sesgos:** reproducen prejuicios presentes en los datos de entrenamiento.
- **Privacidad:** riesgo si se introducen datos sensibles.
- **Actualización:** algunos modelos no tienen acceso a información en tiempo real.
- **Dependencia:** pueden fomentar exceso de confianza si no se validan resultados.

---

## Herramientas destacadas

### ChatGPT (OpenAI)
- **Fortalezas:** generación de contenido creativo y estructurado, razonamiento general, ecosistema de integraciones.
- **Usos en PYMEs:** redacción de emails, creación de manuales, generación de posts para redes sociales.
- **Limitaciones:** puede inventar datos; requiere supervisión.

### Perplexity
- **Fortalezas:** respuestas con citas y enlaces, orientado a búsqueda y verificación.
- **Usos en PYMEs:** investigación de mercado, recopilación de información con fuentes.
- **Limitaciones:** depende de la calidad de las fuentes indexadas.

### Gemini (Google)
- **Fortalezas:** integración con productos Google, capacidades multimodales (texto, imagen, audio).
- **Usos en PYMEs:** documentación en Google Docs, análisis de hojas de cálculo, generación de presentaciones.
- **Limitaciones:** acceso condicionado a cuentas y planes; privacidad según políticas de Google.

---

## Prompt Engineering: cómo hablar con la IA
El **prompt** es la instrucción que damos al modelo. La calidad del resultado depende en gran medida de cómo lo formulamos.

### Principios básicos
1. **Claridad:** especificar contexto, rol, audiencia y objetivo.
2. **Estructura:** dividir en pasos o requisitos claros.
3. **Formato:** indicar cómo queremos la salida (tabla, lista, email).
4. **Iteración:** refinar el prompt según el resultado.
5. **Verificación:** comprobar exactitud y relevancia.

### Ejemplo de prompt eficaz

#### Actúa como un empleado de marketing digital. Redacta un email de 150 palabras para PYMEs en Madrid, presentando un nuevo servicio de consultoría en IA. Incluye 3 beneficios claros, tono profesional y una llamada a la acción.


---

## Buenas prácticas de uso en PYMEs
- **No introducir datos sensibles:** proteger información de clientes y empleados.
- **Revisión humana:** validar antes de enviar o publicar.
- **Uso responsable:** transparencia en contenidos generados con IA.
- **Documentación interna:** crear guías de prompts y políticas de uso.
- **Medición de impacto:** evaluar tiempo ahorrado, calidad y satisfacción.

---

## Conexión con el trabajo final
Los aprendizajes de este módulo se integran en:
- **Guía de prompts corporativos:** estándar interno para tareas clave.
- **Evaluación comparativa de herramientas:** decidir qué modelo usar en cada área.
- **Política de uso responsable:** marco de gobernanza para la digitalización.

# Ejemplos de Prompts por Sector

## Comercio minorista
- **Email de promoción**
  > Actúa como especialista en marketing para comercio minorista.  
  > Redacta un email de 150 palabras dirigido a clientes habituales de una tienda de ropa en Madrid.  
  > Incluye una promoción de temporada (20% descuento), 3 beneficios del producto y una llamada a la acción clara.  
  > Usa un tono cercano y profesional.  

- **Publicación en redes sociales**
  > Genera un post para Instagram de una tienda de alimentación local.  
  > El objetivo es anunciar la llegada de productos ecológicos.  
  > Usa un tono fresco y amigable, incluye 3 hashtags relevantes y una invitación a visitar la tienda.  

---

## Servicios profesionales
- **Documento resumen**
  > Actúa como consultor en transformación digital.  
  > Resume en 300 palabras las principales ventajas de implementar IA en una Pyme de servicios.  
  > Organiza el texto en 3 apartados: eficiencia, innovación y competitividad.  
  > Usa un tono formal y orientado a directivos.  

- **Guion de llamada comercial**
  > Redacta un guion de 2 minutos para una llamada telefónica de una asesoría fiscal a potenciales clientes.  
  > Incluye: presentación breve, 3 beneficios del servicio, ejemplo de ahorro y cierre con invitación a reunión.  
  > Usa un tono profesional y persuasivo.  

---

## Industria ligera
- **Informe técnico**
  > Actúa como ingeniero de procesos.  
  > Redacta un informe de 400 palabras sobre cómo la IA puede optimizar la gestión de inventario en una empresa de fabricación de muebles.  
  > Incluye ejemplos de predicción de demanda, reducción de costes y mejora en tiempos de entrega.  
  > Usa un tono técnico y estructurado.  

- **Ideas de innovación**
  > Genera 5 ideas innovadoras para aplicar IA en un taller mecánico de tamaño medio.  
  > Clasifica las ideas en: atención al cliente, gestión de repuestos, mantenimiento predictivo, formación de empleados y marketing.  
  > Usa un formato de lista con explicación breve de cada idea.  


# Casos de uso de IA por sector en PYMEs

| Sector              | Casos de uso principales                                                                 | Ejemplos prácticos                                                                 |
|---------------------|------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------|
| **Comercio minorista** | - Marketing y promociones<br>- Atención al cliente<br>- Gestión de inventario           | - Emails de ofertas personalizadas<br>- Chatbots para consultas<br>- Predicción de demanda |
| **Servicios profesionales** | - Documentación y reporting<br>- Captación de clientes<br>- Formación interna        | - Resúmenes de informes<br>- Guiones de llamadas comerciales<br>- Microcursos generados con IA |
| **Industria ligera** | - Optimización de procesos<br>- Mantenimiento predictivo<br>- Innovación de producto     | - Análisis de inventario<br>- Alertas de fallos en maquinaria<br>- Generación de ideas de mejora |


#### Ejercicios

##### Ejercicio 1.2 A

- Objetivo: Crear una guía interna de prompts reutilizables para 3 áreas (p. ej., ventas, marketing, atención).

- Pasos:

1. Definir 3 tareas clave por área: ejemplo: “redactar email de propuesta”, “resumir feedback de clientes”, “generar post de LinkedIn”.

2. Diseñar prompts base con variables:

- Prompt tipo: “Actúa como [rol]. Para [audiencia], redacta [tipo de contenido] con tono [tono], usando estos datos: [datos]. Entrega en [formato], con [criterios de calidad].”

3. Probar en ChatGPT, Perplexity, Copilot y Gemini: comparar resultados y refinar.

4. Documentar versiones: prompt v1, v2 y mejoras (qué cambió y por qué).

- Entregable para el trabajo final: “Guía de prompts corporativos v1” con 9 prompts (3 áreas × 3 tareas) y notas de uso.

##### Ejercicio 1.2 B

- Objetivo: Esbozar una política breve de 1–2 páginas para el uso interno de IA.

Contenido mínimo:

- Privacidad y datos: qué datos se permiten, anonimización, no subir información sensible.

- Revisión humana: cuándo es obligatoria antes de uso externo.

- Transparencia: cuándo declarar uso de IA en contenidos públicos.

- Calidad y control: checklist de verificación; fuentes y evidencias.

- Cumplimiento legal: propiedad intelectual, derechos de autor, marca y confidencialidad.

- Entregable para el trabajo final: “Política interna de IA v1” aprobada por dirección.


