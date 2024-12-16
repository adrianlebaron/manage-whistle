# Netlify Forms
### La funcionalidad de Netlify para manejar formularios sin servidor te permite manejar tus formularios sin llamadas API extras o Javascript adicional
1. Sigue este doc de Netlify para que aprendas a detalle cómo activar la detección de formularios en tus sitios en tu dashboard de Netlify, ahí también explica más detalles sobre cómo crear formularios de HTML y Javascript con AJAX y más 👉 [Forms setup](https://docs.netlify.com/forms/setup/?_gl=1%2a1bsh0js%2a_gcl_au%2aOTc5MDY2NzU4LjE3MjkxMTM4Njg)
🤚Despues de que le eches un vistazo a ese doc de Netlify regresa a esta guía para continuar!
2. El único detalle que no incluye explicitamente el doc de Netlify es que para que nuestros formularios en React JSX sean detectados por Netlify, es que, debemos agregar el formulario a nuestro `index.html` también.
3. Por ejemplo: tenemos un formulario de contacto > `ContactForm.jsx` que es el componente con el que va a interactuar el usuario en la página.
4. Debes agregar este input escondido 👉 `<input type="hidden" name="form-name" value="form" />` como en la línea 5 del ejemplo de abajo
```jsx title="TestForm.jsx" hl_lines="4-23" linenums="1"
function testForm() {
    return (
        <>
            <form name="contact" method="post" data-netlify="true">
                <input type="hidden" name="form-name" value="form" />
                <p>
                    <label>Your Name: <input type="text" name="name" /></label>
                </p>
                <p>
                    <label>Your Email: <input type="email" name="email" /></label>
                </p>
                <p>
                    <label>Your Role: <select name="role[]" multiple>
                        <option value="leader">Leader</option>
                        <option value="follower">Follower</option>
                    </select></label>
                </p>
                <p>
                    <label>Message: <textarea name="message"></textarea></label>
                </p>
                <p>
                    <button type="submit">Send</button>
                </p>
            </form>
        </>
    )
}

export default testForm
```
Netlify no va a detectar nuestro formulario de JSX ahí, así que, debemos agregarlo también en `index.html` para que lo detecte. Y la estructura de nuestro proyecto de React es:
```
|-- src/ 
|   |-- components/
|   |   |-- ContactForm.jsx
|
|-- index.html
```
4. Necesitas agregar tu formulario dentro de la etiqueta `<body> </body>` en `index.html`, aunque no es necesario incluir todas las etiquetas envoltorias extra, por ejemplo así:

```html title="index.html" hl_lines="12-17"
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <link rel="icon" type="image/svg+xml" href="/favicon-square.png" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Test Form Site</title>
</head>

<body>
  <form data-netlify="true" netlify name="test-form" method="post" hidden>
    <input type="text" name="name" />
    <input type="email" name="email" />
    <select name="role[]" multiple></select>
    <textarea name="message"></textarea>
  </form>
  <div id="root"></div>
  <script type="module" src="/src/main.jsx"></script>
</body>

</html>
```
Debes incluir los atributos o propiedades correctas a las etiquetas y los mismos nombres de los inputs que pusiste en el formulario de `JSX`
Eso es todo, ya solo debes lanzar tu sitio en Netlify para que pruebes si el formulario es detectado por Netlify y todo lo demás relacionado a eso como activar notificaciones, ver los envíos, entre otras cosas como viste en el doc de Netlify que puse al principio en esta guía👍😉