>[DIAPOSITIVAS](S2-recursos/etiquetas-semanticas.pdf)

---


Las últimas etiquetas que vamos a ver en la sesión de hoy son las etiquetas semánticas, cuyo objetivo es que los motores de búsqueda entiendan mucho mejor nuestra estructura y contenido de la web y posicionarla de una manera más eficaz. 

## HEADER

Hace referencia al título de nuestra página web y contenido importante que hiciese referencia a nuestra página.

```html
<header>
	<!-- Título de nuestra página y contenido importante sobre ella-->
</header>
```

## NAV

Sección de nuestro documento HTML donde encapsularíamos la navegación, lo que viene siendo el menu de la página.

```html
<nav>
	<!-- Navegación de la página-->
</nav>
```

## SECTION

Etiqueta que utilizaremos para estructurar cada una de las secciones de nuestra página web. Si tomamos como referencia un periódico, estas serían la sección noticias, sección deportes…

```html
<section>
	<!-- Bloque de contenidos-->
</section>
```

## ARTICLE

Los article podemos identificarlos, siguiendo el símil, como cada una de los artículos de esas secciones del periódico. Hace referencia a una parte de código que puede ser independiente.

Estos artículos nos los podríamos llevar a cualquier lado de la página web y seguirían teniendo significado propio.

```html
<article>
	<!-- Contenido con significado propio -->
</article>
```

## ASIDE

Para indicar contenido no prioritario, como podría ser la sección de anuncios.

```html
<aside>
	<!-- Contenido no prioritario -->
</aside>
```

## FOOTER

Sería el pie de página de nuestra web.

```html
<footer>
	<!-- Pie de página -->
</footer>
```

El ejemplo que hemos trabajado:

 

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>El periódico de Edu</title>
</head>
<body>
    <!-- Cabecera de la página web -->
    <header>
        <h1>El periódico de Edu</h1>
        <p>Las noticias que estabas buscando</p>
    </header>
    <hr>
    <!-- Sección de últimas noticias destacadas -->
    <section>
        <h2>Sección últimas noticias</h2>
        <!-- Artículo 1 -->
        <article>
            <h3>Noticia 1</h3>
            <p> Descripción noticia 1</p>
        </article>
        <!-- Artículo 2 -->
        <article>
            <h3>Noticia 2</h3>
            <p> Descripción noticia 2</p>
        </article>
        <!-- Artículo 3 -->
        <article>
            <h3>Noticia 3</h3>
            <p> Descripción noticia 3</p>
        </article>
    </section>
    <hr>
    <!-- Sección de deportes -->
    <section>
        <h2>Sección deportes</h2>
        <!-- Artículo 1 -->
        <article>
            <h3>Noticia 1</h3>
            <p> Descripción noticia 1</p>
        </article>
        <!-- Artículo 2 -->
        <article>
            <h3>Noticia 2</h3>
            <p> Descripción noticia 2</p>
        </article>
        <!-- Artículo 3 -->
        <article>
            <h3>Noticia 3</h3>
            <p> Descripción noticia 3</p>
        </article>
    </section>
    <hr>
    <!-- Sección de anuncios (contenido no relevante semanticamente) -->
    <aside>
        <p>Anuncio 1</p>
        <p>Anuncio 2</p>
    </aside>
    <!-- Pie de la web -->
    <footer> Todo los derechos pertenecen a Fulanito</footer>
</body>
</html>
```
