# Guía: Flujo Automático con Make.com
### Google Forms → Router → Gmail + Telegram / Gmail + Google Sheets

Este flujo clasifica consultas entrantes de clientes y responde automáticamente según su urgencia.

```
Google Forms
      ↓
   Make.com
      ↓
  [ROUTER - lógica condicional]
   ↙              ↘
URGENTE          NORMAL
   ↓                ↓
Gmail           Gmail
(respuesta      (respuesta
 prioritaria)    estándar)
   +                +
Telegram        Google Sheets
(alerta         (registro
 al dueño)       del lead)
```

---

## Herramientas necesarias

| Herramienta | Para qué | Coste |
|---|---|---|
| Make.com | Orquestador del flujo | Free (1.000 ops/mes) |
| Google Forms | Trigger de entrada | Gratis |
| Gmail | Respuestas automáticas | Gratis |
| Google Sheets | Base de datos de leads | Gratis |
| Telegram | Alerta al propietario | Gratis |

---

## ANTES DE ENTRAR EN MAKE

### Paso 1 — Crea el Google Form

Ve a [forms.google.com](https://forms.google.com) y crea un formulario con estos campos exactos:

| Campo | Tipo |
|---|---|
| Nombre | Respuesta corta |
| Email | Respuesta corta |
| Tipo de consulta | Desplegable: `Presupuesto` / `Incidencia urgente` / `Información general` |
| Mensaje | Párrafo |

Deja el formulario abierto en otra pestaña.

### Paso 2 — Crea la Google Sheet

En [sheets.google.com](https://sheets.google.com) crea una hoja nueva con estas cabeceras exactas en la fila 1:

```
Fecha | Nombre | Email | Tipo | Mensaje | Estado
```

### Paso 3 — Configura Telegram

Necesitas dos cosas: un **Bot Token** y tu **Chat ID**.

#### 3a. Crea el bot y obtén el Token

1. Abre Telegram y busca `@BotFather`
2. Escríbele `/newbot`
3. Sigue las instrucciones: ponle un nombre y un username (debe acabar en `_bot`)
4. Al finalizar recibirás un **Token** con este formato:
   ```
   7123456789:AAFxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
   ```
5. Copia y guarda ese Token, lo necesitarás en el Paso 16

#### 3b. Obtén tu Chat ID

**Método A — con @userinfobot (más rápido):**
1. Busca `@userinfobot` en Telegram
2. Escríbele cualquier mensaje (un punto, un "hola")
3. Te responderá con tu `Id:` numérico. Ese es tu Chat ID

**Método B — con el navegador (si @userinfobot no responde):**
1. Primero manda cualquier mensaje a tu nuevo bot
2. Abre esta URL en el navegador sustituyendo tu token:
   ```
   https://api.telegram.org/bot[TU_TOKEN]/getUpdates
   ```
3. En el JSON que aparece busca esta estructura:
   ```json
   "chat":{"id": 123456789
   ```
4. Ese número es tu Chat ID

---

## EN MAKE.COM

### Paso 4 — Crea una cuenta

Ve a [make.com](https://make.com) → Sign up gratis → Confirma el email.

### Paso 5 — Crea un escenario nuevo

Panel principal → `Create a new scenario` → botón `+` en el centro del lienzo.

---

## MÓDULO 1 — TRIGGER: Google Forms

### Paso 6 — Añade el módulo Google Forms

Haz clic en `+` → busca `Google Forms` → selecciona **Watch Responses**

### Paso 7 — Conecta tu cuenta Google

Haz clic en `Add` cuando te pida conexión → autoriza con tu cuenta Google.

### Paso 8 — Configura el módulo

- **Form ID:** selecciona el formulario que creaste en el Paso 1
- **Limit:** `1`

Haz clic en `Save`. Make te preguntará `Choose where to start` → selecciona **From now on**.

> ⚠️ **Importante sobre el mapeo de campos:** Google Forms envía los datos en formato JSON anidado. Cuando mapees campos en los módulos siguientes, siempre despliega el campo hasta el nivel más profundo y selecciona **`value`**. La ruta completa será: `Answers > [Campo] > textAnswers > answers > value`. Si no llegas al `value`, el campo mostrará JSON crudo en lugar del texto del usuario.

---

## MÓDULO 2 — ROUTER

### Paso 9 — Añade el Router

Haz clic en el círculo de la derecha del módulo de Forms → busca `Router` → selecciónalo.

El Router aparece en el lienzo con dos rutas vacías.

---

## RUTA A — URGENTE

### Paso 10 — Configura la condición de la Ruta A

Haz clic en la llave inglesa ⚙️ sobre la línea de la Ruta A → `Set up a filter`

```
Label:     Urgente
Condition: Answers > Tipo de consulta > value   Equal to   Incidencia urgente
```

> Recuerda expandir hasta `value` para que la condición compare texto limpio.

### Paso 11 — Añade Gmail (email urgente)

Clic en `+` de la Ruta A → `Gmail` → **Send an Email** → conecta tu cuenta Google.

Rellena los campos mapeando siempre hasta el nivel `value`:

```
To:      Answers > Email > value
Subject: Tu consulta urgente ha sido recibida — te contactamos hoy
Body:    [Nombre], hemos visto tu mensaje y lo estamos atendiendo como prioritario.
         Un responsable se pondrá en contacto contigo antes de las próximas 4 horas laborables.

         Asunto de tu consulta: [Mensaje > value]

         Quedo a tu disposición,
         [Tu nombre / empresa]
```

> En Body type selecciona **Plain text**.

### Paso 12 — Añade Telegram Bot (alerta al propietario)

Clic en `+` después del Gmail de la Ruta A → busca `Telegram Bot` → **Send a Text Message or a Reply**

Haz clic en `Add` para crear la conexión → te pedirá el **Token** del bot que creaste en el Paso 3a. Pégalo y guarda.

Rellena:

```
Chat ID:  [Tu Chat ID del Paso 3b]
Text:     ⚠️ URGENTE: [Nombre > value] | [Email > value] | [Mensaje > value]
```

---

## RUTA B — NORMAL

### Paso 13 — Condición de la Ruta B

Haz clic en la llave inglesa de la Ruta B → `Set up a filter`

```
Label: Normal
```

**No añadas ninguna condición** — esto la convierte en ruta por defecto (todo lo que no sea urgente cae aquí automáticamente).

### Paso 14 — Añade Gmail (email estándar)

Clic en `+` de la Ruta B → `Gmail` → **Send an Email**

```
To:      Answers > Email > value
Subject: Hemos recibido tu consulta, [Nombre > value]
Body:    Gracias por escribirnos. Hemos anotado tu consulta sobre
         [Tipo de consulta > value] y te responderemos en un plazo
         máximo de 24 horas.

         Si necesitas atención más rápida, responde a este email indicándolo.

         El equipo de [empresa]
```

> En Body type selecciona **Plain text**.

### Paso 15 — Añade Google Sheets (registro del lead)

Clic en `+` después del Gmail de la Ruta B → `Google Sheets` → **Add a Row**

Conecta tu cuenta → selecciona la hoja `Leads entrantes`.

Mapea columna a columna (recuerda llegar siempre hasta `value`):

```
Fecha:    {{now}}
Nombre:   Answers > Nombre > value
Email:    Answers > Email > value
Tipo:     Answers > Tipo de consulta > value
Mensaje:  Answers > Mensaje > value
Estado:   Pendiente   ← texto fijo, sin mapear
```

---

## ACTIVAR Y PROBAR

### Paso 16 — Guarda el escenario

Botón `Save` abajo a la izquierda.

### Paso 17 — Activa el escenario

El toggle abajo a la izquierda que pone `OFF` → ponlo en `ON`. A partir de ahora el escenario está escuchando respuestas nuevas.

### Paso 18 — Prueba la Ruta A (Urgente)

1. Abre el formulario y rellena todos los campos con un email real
2. En `Tipo de consulta` selecciona **Incidencia urgente**
3. Envía el formulario
4. Espera 30-60 segundos
5. Comprueba que llega el email **y** el mensaje de Telegram

### Paso 19 — Prueba la Ruta B (Normal)

1. Rellena el formulario con `Tipo de consulta: Presupuesto`
2. Envía
3. Comprueba el email y que aparece una nueva fila en Google Sheets

---

## SOLUCIÓN DE PROBLEMAS FRECUENTES

| Síntoma | Causa | Solución |
|---|---|---|
| Los campos muestran JSON crudo en el email | El mapeo coge el objeto completo, no el valor | Despliega el campo hasta el nivel `value` |
| El escenario no detecta respuestas | Make ya procesó esas respuestas antes | Envía una respuesta **nueva** con el escenario activo |
| Error "Invalid email address in parameter 'to'" | El campo Email llega vacío o el mapeo es incorrecto | Verifica que llegas a `value` en el mapeo del campo Email |
| Telegram no recibe el mensaje | Token o Chat ID incorrectos | Verifica el Token sin espacios y el Chat ID con el método del navegador |
| Google Sheets da error de columnas | Las cabeceras no coinciden con el mapeo | Comprueba que las cabeceras de la fila 1 son exactamente: Fecha, Nombre, Email, Tipo, Mensaje, Estado |

---

## NOTAS PARA AMPLIAR EL FLUJO

Una vez que el flujo base funciona, estos son los siguientes pasos naturales para hacerlo más potente:

- **Añadir IA en el bucle:** Insertar un módulo HTTP que llame a la API de OpenAI o Claude entre el Forms y el Gmail para que la respuesta sea generada dinámicamente según el mensaje del cliente
- **Añadir condición por palabras clave:** Ampliar el Router con una tercera ruta que detecte palabras como "cancelar", "baja" o "queja" para tratarlas de forma específica
- **Notificación a Slack o Teams:** Sustituir o añadir junto a Telegram un módulo de Slack/Teams si el equipo trabaja en esas plataformas
- **CRM básico en Sheets:** Añadir una columna `Seguimiento` con fecha y estado para convertir la hoja en un pipeline de ventas simple