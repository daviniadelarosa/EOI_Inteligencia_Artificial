# 5.4 Organización y análisis de datos internos con IA

## 1. El Concepto: De la "Carpeta de Archivos" al "Cerebro Semántico"
Tradicionalmente, las empresas organizan su información de forma jerárquica (Carpetas > Subcarpetas > Archivos). El problema es que si no sabes dónde guardaste algo, todo se complica.

- La Revolución: Con la IA, pasamos a la búsqueda semántica. Ya no buscamos por "nombre de archivo", sino por "concepto".

- El "Cerebro Interno": Consiste en alimentar a una IA privada con toda la base de conocimiento de la empresa (leyes, convenios, contratos antiguos, circulares de Hacienda) para que cualquier empleado pueda preguntarle dudas complejas, como ya hemos visto en todas las sesiones anteriores.

## 2. Organización Inteligente de Datos (Estructuración)

### A. La Teoría: Del "Dark Data" a la Información Accionable
El mayor problema en una empresa, no es la falta de datos, sino que sus datos no están "limpios" (Dark Data). Son archivos que ocupan espacio pero cuya información no se puede buscar, filtrar ni operar con ella fácilmente.

- Datos No Estructurados (80%): Son "fotos" de la realidad. Un PDF de una escritura, un audio de un cliente por WhatsApp diciendo "cambia mi cuenta bancaria", o un email con una duda fiscal. Para un ordenador tradicional, esto es solo un montón de píxeles o bytes sin sentido.

- La IA como "Traductor Universal": La IA moderna utiliza LLMs (Large Language Models) combinados con OCR Inteligente (Reconocimiento Óptico de Caracteres). No solo "lee" las letras, sino que entiende el contexto. Sabe distinguir si un número es un código postal, un NIF o una base imponible simplemente por su posición y significado en el documento.

### B. Aplicación en la Gestoría: Clasificación y Triaje Automático
En una gestoría, el "cuello de botella" es la entrada de documentos. La IA transforma este proceso de manual a automático:

1. Reconocimiento de Patrones Semánticos:

- La IA identifica el tipo de documento sin que nadie se lo diga. Si detecta la palabra "Censo", "Actividad" y un código de barras específico, etiqueta el archivo como "Modelo 036".

- Si ve "Base Imponible", "Cuota" y "Fecha de Vencimiento", lo etiqueta como "Factura de Proveedor".

2. Extracción de Metadatos (La "Magia" de la IA):

- No se limita a guardar el PDF. "Extrae" los datos clave.

- Ejemplo: Del contrato de alquiler de un autónomo, la IA extrae: Fecha de fin de contrato, Renta mensual y Fianza.

- El Valor: El sistema puede crear una alerta en el calendario del gestor: "Aviso: El alquiler del cliente Juan Pérez vence en 30 días, hay que renovarlo". El gestor nunca abrió el archivo; la IA lo hizo por él.

3. Enrutamiento Inteligente:

- Una vez clasificado, la IA puede saber dónde va. No hace falta que un administrativo mueva el archivo a la carpeta 2026 > Clientes > Marta García > Impuestos. La IA crea la carpeta si no existe y lo deposita allí con un nombre normalizado: 2026_M036_MartaGarcia.pdf, si tenemos todo esto correctamente automatizado.

### C. Limpieza y Reconciliación de Datos (El "Detective" de Errores)
Las bases de datos de las empresas pequeñas suelen estar llenas de "ruido" (errores). La IA actúa como un "auditor" que no se cansa.

- Detección de Inconsistencias: La IA cruza datos. Si en el Modelo 036 el NIF del cliente termina en "B", pero en una factura emitida por él termina en "V", la IA lanza una alerta inmediata: "Posible error de dedo en la factura nº 45, el NIF no coincide con el registro oficial".

- Unificación de Identidades (Deduplicación):

Es común tener al mismo cliente registrado como "Marta García", "Marta Gª" y "Marta García S.L.".

La IA analiza el contexto (dirección, NIF, teléfono) y propone: "He encontrado 3 fichas que parecen ser la misma persona. ¿Quieres unificarlas en una sola ficha de cliente?". Esto limpia el CRM y evita duplicar cobros o comunicaciones.

- Detección de "Huecos" de Información:

La IA puede analizar la carpeta de un autónomo y avisar: "Falta el certificado de estar al corriente de pago de este trimestre para el cliente X, y es necesario para su licitación de mañana".

### D. Por qué esto es importante
La estructuración de datos es la base para todo lo demás.

"Si los datos están desordenados, la IA solo ayudará a cometer errores más rápido. Pero si usas la IA para organizar tus datos, pasarás de ser 'recolector de papeles' a ser 'analista de información'. El valor para los clientes ya no será guardar sus facturas, sino decirle qué significan esas facturas para su negocio."

### E. Resumen:

- Captura: La IA "ve" y "entiende" el documento (PDF, imagen, email).

- Extracción: Convierte el texto del documento en datos (Nombres, fechas, importes).

- Validación: Comprueba si los datos son correctos y no están duplicados.

- Acción: Guarda, avisa o rellena el Excel/Software contable.

## 3. Análisis de Datos: Del "Qué pasó" al "Qué pasará"
El análisis tradicional es descriptivo (mirar el balance de ayer), aunque esto ha ido cambiando con el tiempo. El análisis con IA es predictivo y prescriptivo (nos dice qué va a pasar y qué debemos hacer).

**Aplicación en la Gestoría:**
1. Detección de Patrones de Ahorro Fiscal:

- La IA analiza todos los gastos de un autónomo durante el año y los compara con otros del mismo sector.

- Resultado: "He detectado que este diseñador gráfico no está deduciendo el pocentaje correspondiente de sus suministros de hogar a pesar de trabajar en casa. Podría ahorrar dinero extra este trimestre".

2. Análisis de Riesgo de Abandono (Churn):

- La IA analiza el tono de los emails y la frecuencia de contacto.

- Resultado: "Este cliente lleva dos meses enviando las facturas tarde y su tono en los emails es de insatisfacción. Riesgo alto de que se vaya a otra gestoría. Sugerencia: Llamada de fidelización hoy".

3. Auditoría de Errores antes de Hacienda:

- Antes de enviar el trimestre, la IA cruza todos los datos.

- Resultado: "Atención: El total de IVA soportado no cuadra con las facturas digitalizadas. Falta una factura de 1.200€ o hay un error de suma en el asiento".

## 4. Algunas herramientas

| Herramienta              | Función en la Gestoría |
|--------------------------|-------------------------|
| NotebookLM (Google)      | Subes todos los manuales de la AEAT y convenios colectivos. Los empleados le preguntan dudas legales y la IA responde citando la fuente exacta. |
| ChatGPT Data Analyst     | Subes el Excel de facturación de toda la gestoría para ver qué tipo de cliente es el más rentable y cuál da más trabajo. |
| Claude (con Projects)    | Creas un "espacio de trabajo" con los contratos tipo de la gestoría. Le pides: "Redacta un nuevo contrato para un cliente de servicios digitales basándote en nuestro estilo estándar". |

## 5. El Valor Estratégico: La Pyme que "Sabe lo que Sabe"
El mayor activo de su Pyme no es su local, sino su información.

- Memoria Institucional: Si el gestor senior se jubila, su conocimiento (cómo trataba a X cliente, qué trucos legales usaba) se queda en el "Cerebro IA" de la empresa.

- Toma de decisiones basada en datos, no en intuición: Ya no dicen "creo que este mes vamos mal", dicen "la IA muestra una caída del 12% en servicios de consultoría, vamos a lanzar una oferta".

## Ejercicio

A partir de este dataset de ejemplo:

```csv
Fecha,Concepto,Categoría,Ingreso,Gasto,IVA_Soportado
02/01/2026,Diseño Web Cliente A,Servicios,1200,0,252
05/01/2026,Compra Ordenador Pro,Suministros,0,1500,315
10/01/2026,Publicidad Meta Ads,Marketing,0,200,42
15/01/2026,Asesoría Mensual,Gestoría,0,60,12.6
20/01/2026,Logotipo Cliente B,Servicios,500,0,105
25/01/2026,Seguro Responsabilidad Civil,Seguros,0,250,0
02/02/2026,Mantenimiento Web C,Servicios,300,0,63
05/02/2026,Suscripción Adobe,Software,0,60,12.6
10/02/2026,Cena Cliente (Injustificada),Varios,0,85,17.85
15/02/2026,Asesoría Mensual,Gestoría,0,60,12.6
18/02/2026,Suscripción Canva,Software,0,12,2.52
28/02/2026,Consultoría Estratégica,Servicios,2000,0,420
03/03/2026,Alquiler Coworking,Local,0,300,63
05/03/2026,Suscripción Adobe (Duplicada),Software,0,60,12.6
10/03/2026,Internet y Móvil,Suministros,0,50,10.5
15/03/2026,Asesoría Mensual,Gestoría,0,60,12.6
20/03/2026,Diseño Web Cliente D,Servicios,1200,0,252
25/03/2026,Viaje Tren (Sin Factura),Varios,0,120,0
01/04/2026,Mantenimiento Web C,Servicios,300,0,63
05/04/2026,Suscripción Adobe,Software,0,60,12.6
10/04/2026,Publicidad Google Ads,Marketing,0,300,63
15/04/2026,Asesoría Mensual,Gestoría,0,60,12.6
20/04/2026,Campaña Email Marketing,Servicios,800,0,168
28/04/2026,Formación IA Pymes,Servicios,1500,0,315
02/05/2026,Mantenimiento Web C,Servicios,300,0,63
05/05/2026,Suscripción Adobe,Software,0,60,12.6
10/05/2026,Reparación Pantalla Móvil,Suministros,0,180,37.8
15/05/2026,Asesoría Mensual,Gestoría,0,60,12.6
25/05/2026,Alquiler Sala Eventos,Local,0,150,31.5
30/05/2026,Consultoría Estratégica B,Servicios,2500,0,525

```
### A. Instrucciones:
Copia el bloque de arriba y pegalo en ChatGPT o similar (o sube el archivo si usas una versión con licencia).

Dale este contexto: "Soy el dueño de una pequeña gestoría/agencia digital. Analiza estos movimientos del primer semestre y no respondas todavía, solo dime si los entiendes".

### B. Preguntas de Análisis: Ejemplos de preguntas que puedes usar y/o ampliar
1. Detección de Anomalías (Ahorro de dinero):

"Revisa los gastos de 'Software'. ¿Ves alguna irregularidad o algo que debería revisar para no perder dinero?"


2. Análisis Fiscal (Seguridad):

"Actúa como un alguien con conocimientos de contabilidad. Revisa la columna de 'Concepto' y 'IVA_Soportado'. ¿Qué gastos crees que me darán problemas en una inspección de Hacienda?"


3. Tendencias de Negocio (Estrategia):

"¿Cuáles son mis dos servicios más rentables y qué mes ha sido el más flojo en ingresos?"

4. Proyección de futuro:

"Si sigo con este nivel de gastos fijos y esta media de ingresos, ¿cuál será mi beneficio estimado al final del año?"


[Dataset_Ejemplo](https://www.kaggle.com/datasets/kyanyoga/sample-sales-data/data)

[Video](https://www.youtube.com/watch?v=4j9E2zLup5g)
