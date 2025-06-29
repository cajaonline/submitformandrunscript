# CajaOnline — submitFormAndRunScript

🚀 Propuesta experimental de tecnología web para ejecutar código JavaScript de forma segura, temporal y controlada desde el backend.

## 🔍 Objetivo

Simular una API nativa de navegador llamada:

```js
submitFormAndRunScript(formElement, url)
La función:

Envía un formulario vía POST.

Recibe un script JS como respuesta.

Ejecuta el script en un contexto efímero.

El código se elimina automáticamente sin exponerlo en consola ni DOM.

🧪 Archivos incluidos
Archivo	Descripción
index.html	Interfaz de prueba con botón y formulario.
ejecutar.php	Devuelve dinámicamente código JavaScript.
script_dinamico.js	Función auxiliar que recibe, evalúa y borra el JS.

✅ Cómo funciona
Al presionar el botón del formulario, se llama a submitFormAndRunScript.

Esta función hace un POST a ejecutar.php.

El PHP genera un <script> con lógica oculta (no persistente).

El navegador lo ejecuta y lo elimina automáticamente.

🔐 Seguridad
Este sistema:

Evita exponer código sensible en consola.

No deja rastros permanentes en el DOM.

Es útil para ejecutar una única vez instrucciones sensibles como tokens, claves temporales, redireccionamientos, etc.

⚠️ Advertencia
Esta tecnología es experimental y no estándar.
No reemplaza mecanismos seguros como CORS, CSP o APIs nativas.
Fue creada con fines de demostración y exploración.

📜 Licencia
Uso privado no comercial.
Autor: Dante Mariano Tomasini — MSMG Informática.
