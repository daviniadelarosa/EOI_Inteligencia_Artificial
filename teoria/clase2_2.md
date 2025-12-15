# Cómo enviar un email HTML desde Gmail sin que se "pierda" el diseño

## 1. Abre Gmail y crea un nuevo correo
Haz clic en Redactar.

## 2. Copia el HTML desde un navegador, no desde un editor
Gmail no acepta pegar código HTML directamente.
Necesitas pegar el resultado visual, no el código.

- Tienes dos opciones:

### ✅ OPCIÓN A (la más fácil): Usar una vista previa en el navegador

1. Abre un archivo nuevo en tu ordenador (por ejemplo, email.html).
2. Pega dentro el HTML que te di.
3. Guarda el archivo.
4. Ábrelo en tu navegador (Chrome, Edge, etc.).
5. Selecciona todo el contenido visual (Ctrl+A o Cmd+A).
6. Copia (Ctrl+C o Cmd+C).
7. Pega directamente en el cuerpo del email de Gmail.

✅ Gmail mantendrá los estilos inline perfectamente.

### ✅ OPCIÓN B: Usar una herramienta online (si no quieres crear archivos)
- Puedes usar un visor HTML online como:
[html-online.com/editor/](html-online.com/editor/)
[codebeautify.org/htmlviewer](codebeautify.org/htmlviewer)

Pasos:

1. Pega el HTML en el editor.
2. Mira la vista previa.
3. Selecciona la vista previa completa.
4. Copia y pega en Gmail.

### ✅ OPCIÓN C: Usar extensiones (si lo haces a menudo)

Hay extensiones como:

- Gmail Email Templates
- Gmail HTML Inserter

Permiten pegar HTML directamente, pero no son necesarias si solo envías un email puntual.

✅ IMPORTANTE: Qué NO debes hacer
❌ No pegues el código HTML directamente en Gmail.
Gmail lo interpreta como texto y lo rompe.

❌ No uses estilos en <style> porque Gmail los elimina.
Por eso te preparé el email con estilos inline, que sí respeta.