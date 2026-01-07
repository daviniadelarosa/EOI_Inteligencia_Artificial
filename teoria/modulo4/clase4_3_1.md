# 4.3 Creación de propuestas de venta automatizadas y personalizadas
## 1. El Concepto: De la Propuesta Reactiva a la Proactiva
La mayoría de las empresas, envían presupuestos sólo cuando se los piden, pero la IA permite crear Propuestas Dinámicas basadas en datos:

Veamos algunos ejemplos: 

- Renovaciones Inteligentes: El sistema detecta que el contrato de un cliente vence en 30 días, analiza qué servicios usó más y le envía una propuesta de renovación personalizada, no un PDF genérico.

- Fidelización (Upselling/Cross-selling): Si un cliente de "Casa Carmen" siempre pide vino tinto caro, la IA puede enviarle una propuesta personalizada para una "Cata Privada" o un menú especial de maridaje.

- Recuperación de Clientes (Win-back): Localizar clientes que no compran hace 6 meses y generar una propuesta que diga: "Sabemos que te encantaba el Chuletón, hemos renovado la carta y tenemos esto para ti...".

## 2. El Flujo de Trabajo (Workflow) Automatizado
Para que esto sea "útil", no puede ser solo manual sobre todo si el número de clientes es relativamente elevado. La idea es tener un Pipeline de Ventas IA.

Veamos en esta tabla un resumen: 

| Fase       | Herramienta (Ecosistema 2025/26)                 | Acción de la IA                                                                                   |
|------------|--------------------------------------------------|----------------------------------------------------------------------------------------------------|
| Detección  | CRM (HubSpot, Pipedrive) o Google Sheets         | Identifica al cliente que cumple el criterio (ej. 1 año desde su última compra).                  |
| Análisis   | GPT-4o / Claude 3.5                              | Lee el historial de pedidos y redacta una propuesta basada en sus gustos reales.                  |
| Generación | Canva Magic Design o Gamma.app                   | Crea un documento visual o presentación web personalizada en segundos.                            |
| Envío      | Make.com o Instantly.ai                          | Envía la propuesta por el canal preferido del cliente (WhatsApp o Email).                         |


### El Pipeline de Ventas con IA: Anatomía de un Proceso "Zero-Touch"

El objetivo es que la Pyme pase de ser solo un "tomador de pedidos" a un "generador de oportunidades" constante.

#### Fase 1: Detección (El Disparador o Trigger)
- No enviamos propuestas a todos, sino a los segmentos calientes.

- Cómo funciona: Configuramos un "vigilante" en nuestra base de datos (CRM o Excel). Este vigilante busca eventos específicos.

- Ejemplos de criterios en 2026: * Inactividad: "Cliente que gastó >500€ el año pasado pero lleva 90 días sin comprar".

- Comportamiento: "Cliente que ha abierto 3 veces el email sobre el nuevo menú de temporada pero no ha reservado".

- Hay herramientas como Zapier o Make.com, que pueden "leer" filas de Google Sheets por ejemplo cada mañana a las 09:00 y, si la fecha de última compra cumple la condición, disparar el resto del proceso.

#### Fase 2: Análisis (La Inteligencia del Contexto)

- Aquí es donde la IA marca la diferencia frente a las automatizaciones antiguas y "frías".

- Uso del historial: La IA no solo sabe el nombre del cliente. Accede al histórico de pedidos. Si el cliente de Casa Carmen siempre pide "Vino tinto" y "Chuletón", el sistema le pasa estos datos a GPT-4o.

- El Prompt interno (Invisible para el cliente): El sistema le dice a la IA: "Analiza estos datos de Juan. Le gusta la carne poco hecha y los vinos de Ribera del Duero. Redacta un párrafo que le invite a probar nuestra nueva 'Entraña de Angus' (14.95€) comparándola con sus gustos habituales".

- Resultado: Una comunicación que parece escrita por el dueño del restaurante que conoce a Juan de toda la vida.

#### Fase 3: Generación (La Propuesta Visual)
- Nadie lee un bloque de texto plano. En 2025/26, las propuestas son experiencias web interactivas.

- Gamma.app / Canva Magic: Estas herramientas permiten recibir el texto analizado en la fase anterior y "volcarlo" en una plantilla predefinida de la empresa.

- Personalización Dinámica: La IA no solo cambia el texto, puede cambiar las fotos. Si la propuesta es para una cena de empresa, Gamma elegirá fotos de grupos; si es para una pareja, fotos de mesas románticas.

- El factor "Wow": El cliente recibe un enlace a una página web personalizada exclusiva para él, con un botón de "Reservar ahora" o "Aceptar presupuesto".

#### Fase 4: Envío y Seguimiento (La Omnicanalidad)
- El último paso es llegar donde está el cliente.

- Make.com como orquestador: Es el "pegamento". Una vez generada la propuesta en Gamma, Make toma el enlace y lo envía.

- Canales inteligentes:

1. WhatsApp (vía API): Si el cliente suele reservar por ahí, se le envía un mensaje corto con el link.

2. Email (Instantly.ai / Lemlist): Si es B2B (empresas), estas herramientas permiten que el email parezca enviado desde tu Gmail personal, evitando la carpeta de promociones.

3. Seguimiento automático: Si el cliente hace clic en el enlace pero no reserva en 24 horas, la IA puede enviar un recordatorio suave: "Hola Juan, ¿viste la propuesta para la cena? Solo nos quedan 2 mesas para ese viernes".

### Ejemplo Real (Basado en el Menú de Casa Carmen)

1. Detección: El Excel de reservas muestra que la "Empresa Tech" no viene desde Navidad.

2. Análisis: La IA lee que en Navidad pidieron 15 "Hamburguesas Ibéricas" y 10 "Tataki de Atún".

3. Generación: Gamma crea automáticamente una mini-web que dice: "Propuesta de Afterwork para Empresa Tech". Incluye fotos de la Hamburguesa Ibérica (del menú) y una oferta especial: "10% de descuento si vuelven a pedir su plato favorito: El Tataki".

4. Envío: Un mensaje automático llega al encargado de la empresa por WhatsApp.

## 3. Herramienta Práctica: Gamma.app (Freemium)

Es una herramienta que genera presentaciones y sitios web de propuestas comerciales a partir de un simple texto.

Pasos a seguir: 

1. Entrar en [Gamma](gamma.app).

2. Elegir "Generate" -> "Presentation" o "Webpage".

3- Introducir el siguiente prompt (instrucción):

**"Crea una propuesta de fidelización para un cliente antiguo del restaurante Casa Carmen. El cliente no viene hace 6 meses, pero antes venía mucho a cenas de empresa. Ofrécele un menú degustación exclusivo para su próxima reunión corporativa basado en sus platos estrella (usar datos del menú PDF)."**

4. Ver cómo la IA diseña toda la propuesta visual en menos de 1 minuto.