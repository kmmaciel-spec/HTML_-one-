# 🌐 Fundamentos de HTML

📚 Aprende a crear la estructura de una página web con etiquetas, ejemplos y ejercicios.

## 🎯 Objetivo

Comprender los conceptos básicos de HTML y crear una página web sencilla.

## 🧠 ¿Qué es HTML?

**HTML** significa **Lenguaje de Marcado de Hipertexto**.

Se utiliza para organizar el contenido de una página web mediante títulos, párrafos, imágenes, enlaces y otros elementos.

HTML es un lenguaje de marcado, no un lenguaje de programación.

| Tecnología | Función |
| --- | --- |
| 🧱 HTML | Estructura y significado del contenido. |
| 🎨 CSS | Diseño, colores y distribución. |
| ⚙️ JavaScript | Lógica e interactividad. |

## 🏗️ Estructura básica

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mi primera página</title>
</head>
<body>
  <h1>¡Hola, mundo! 🌎</h1>
  <p>Estoy aprendiendo HTML.</p>
</body>
</html>
```

### 🔍 ¿Qué hace cada parte?

- `<!DOCTYPE html>`: activa el modo estándar del navegador.
- `<html>`: contiene el documento.
- `lang="es"`: indica que el idioma es español.
- `<head>`: contiene información sobre la página.
- `<meta charset="UTF-8">`: permite interpretar acentos y emojis.
- `<meta name="viewport" ...>`: ajusta el área de visualización en móviles.
- `<title>`: define el título de la pestaña.
- `<body>`: contiene el contenido de la página.

## 🏷️ Etiquetas y atributos

Muchos elementos tienen una etiqueta de apertura, contenido y una etiqueta de cierre:

```html
<p>Este es un párrafo.</p>
```

Los atributos proporcionan información adicional:

```html
<a href="https://developer.mozilla.org/es/docs/Web/HTML">
  Aprende HTML
</a>
```

Aquí, `href` indica el destino del enlace.

📌 Algunos elementos, como `<img>`, `<input>` y `<br>`, no llevan etiqueta de cierre.

## 📝 Encabezados y párrafos

Los encabezados organizan el contenido por niveles, desde `<h1>` hasta `<h6>`.

```html
<h1>Título principal</h1>
<h2>Un tema de la página</h2>
<h3>Un subtema</h3>

<p>Este es un párrafo de texto.</p>
<p>Este contenido es <strong>importante</strong>.</p>
<p>Esta palabra tiene <em>énfasis</em>.</p>
```

💡 Elige los encabezados por su jerarquía, no por su tamaño visual.

## 🔗 Enlaces

Los enlaces permiten navegar hacia otras páginas o secciones.

```html
<a href="https://github.com">Visitar GitHub</a>
```

También puedes enlazar una sección del mismo documento:

```html
<a href="#contacto">Ir a contacto</a>

<section id="contacto">
  <h2>Contacto</h2>
  <p>Gracias por visitar mi página.</p>
</section>
```

## 🖼️ Imágenes

```html
<img
  src="imagenes/paisaje.jpg"
  alt="Montañas junto a un lago al atardecer"
  width="400"
>
```

- `src`: ubicación de la imagen.
- `alt`: alternativa textual que describe la imagen.
- `width`: ancho de visualización en píxeles.

📂 Para usar este ejemplo, coloca `paisaje.jpg` dentro de una carpeta llamada `imagenes`.

## 📋 Listas

### Lista sin orden

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

### Lista ordenada

```html
<ol>
  <li>Crear el archivo.</li>
  <li>Escribir el código.</li>
  <li>Abrirlo en el navegador.</li>
</ol>
```

## 🧩 Etiquetas semánticas

Describen la función del contenido y ayudan a organizar la página.

| Etiqueta | Uso |
| --- | --- |
| `<header>` | Contenido introductorio. |
| `<nav>` | Navegación principal. |
| `<main>` | Contenido principal. |
| `<section>` | Sección temática. |
| `<article>` | Contenido independiente. |
| `<footer>` | Información de cierre. |

## 📊 Tablas

Se utilizan para presentar datos relacionados.

```html
<table>
  <caption>Tecnologías web</caption>
  <thead>
    <tr>
      <th scope="col">Tecnología</th>
      <th scope="col">Función</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>HTML</td>
      <td>Estructurar contenido</td>
    </tr>
    <tr>
      <td>CSS</td>
      <td>Definir la presentación</td>
    </tr>
  </tbody>
</table>
```

## 📬 Formularios

Permiten introducir información mediante campos y botones.

```html
<form>
  <label for="nombre">Nombre:</label>
  <input type="text" id="nombre" name="nombre" required>

  <label for="correo">Correo electrónico:</label>
  <input type="email" id="correo" name="correo" required>

  <button type="submit">Enviar</button>
</form>
```

📌 Este ejemplo muestra la estructura del formulario. Para guardar datos o enviar correos, necesitas conectar un servicio que procese el envío.

## 💬 Comentarios

Los comentarios permiten dejar anotaciones que no aparecen como contenido visible en la página.

```html
<!-- Este es un comentario -->
<p>Este texto sí aparece en la página.</p>
```

## 💻 Ejemplo completo

Guarda este código en un archivo llamado `index.html` y ábrelo en tu navegador.

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Aprendiendo HTML</title>
</head>
<body>
  <header>
    <h1>🌐 Mi primera página web</h1>
    <nav aria-label="Navegación principal">
      <a href="#presentacion">Sobre mí</a>
      <a href="#aprendizaje">Mi aprendizaje</a>
    </nav>
  </header>

  <main>
    <section id="presentacion">
      <h2>👋 Sobre mí</h2>
      <p>Estoy aprendiendo a crear páginas web con HTML.</p>
    </section>

    <section id="aprendizaje">
      <h2>📚 Lo que estoy aprendiendo</h2>
      <ul>
        <li>Crear títulos y párrafos.</li>
        <li>Agregar enlaces e imágenes.</li>
        <li>Organizar el contenido con etiquetas semánticas.</li>
      </ul>
      <a href="https://developer.mozilla.org/es/docs/Web/HTML">
        Consultar la documentación de HTML
      </a>
    </section>
  </main>

  <footer>
    <p>✨ Proyecto de práctica de HTML.</p>
  </footer>
</body>
</html>
```

## ✅ Buenas prácticas

- Usa sangría para organizar el código.
- Cierra las etiquetas que requieren cierre.
- Mantén una jerarquía clara de encabezados.
- Añade alternativas textuales a las imágenes.
- Escribe enlaces descriptivos.
- Relaciona cada campo de formulario con su etiqueta.
- Utiliza HTML semántico.
- Acompaña los emojis con texto.
- Comprueba que la página pueda recorrerse con el teclado.

## 🏆 Actividad práctica

Crea una página personal que incluya:

- [ ] Un título principal.
- [ ] Una presentación breve.
- [ ] Una lista de tres intereses.
- [ ] Una imagen con texto alternativo.
- [ ] Un enlace a un sitio educativo.
- [ ] Un encabezado, contenido principal y pie de página.

## 📚 Recursos

- [Documentación de HTML en MDN](https://developer.mozilla.org/es/docs/Web/HTML)
- [Estándar HTML](https://html.spec.whatwg.org/)
- [Validador de HTML](https://validator.w3.org/nu/)

---

🚀 **¡Aprende, practica y crea tu primera página web!**
