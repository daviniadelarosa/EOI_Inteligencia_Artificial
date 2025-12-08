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


