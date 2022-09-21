>[DIAPOSITIVAS](S2-recursos/etiquetas-de-contenido.pdf)

---


Llega el momento de ver todas aquellas etiquetas que nos van a valer para dar formato a nuestro contenido. Abrimos un nuevo proyecto en VSC y empezamos a trabajar

**HEADING** 

Estas etiquetas nos van a valer para poner títulos en nuestra páginas. Los motores de búsqueda las utilizarán para posicionarse. Podemos utilizar de la etiqueta a ```<h1>``` a la etiqueta ```<h6>``` para estructurar nuestros títulos y subtítulos dentro de la página

 

```html
<h1>Título de la página</h1>
<h2>Subtítulo<h2>
<h3>Sub-subtítulo</h3>
<h4>subsub...</h4>
<h5>subsub...</h5>
<h6>subsub...</h6>
```

 

**PÁRRAFO**

Etiqueta que nos va a permitir escribir contenido dentro de nuestra página web.

```html
<p> Este es mi primer párrafo </p>
```

**SPAN**

Se trata de una etiqueta que nos sirve para contener un trozo del bloque permitiendo aplicarle un formato específico. Por ejemplo, para poder cambiar el estilo de una parte del párrafo usaríamos ```<span>```

```html
<p>Este párrafo es negro. <span style:"color:red;">Y este párrafo es rojo.</span></p>
```

**NEGRITA, SUBRAYADO Y CURSIVA**

Etiquetas que nos van a poder modificar el texto.

- ```<b>``` nos va a permitir poner el bloque que contenga en negrita
- ```<i>``` nos permite poner en cursiva el contenido
- ```<u>``` nos permite poner el bloque que contenga subrayado
- Podemos enfatizar también el texto con la etiqueta ```<strong>```

```html
<p>El siguiente texto va a estar en negrita:<b>Hola Mundo</b></p>
<p>El siguiente texto va a estar en cursiva:<i>Hola Mundo</i></p>
<p>El siguiente texto va a estar en subrayado:<u>Hola Mundo</u></p>
<p>El siguiente texto va a estar en enfatizado:<strong>Hola Mundo</strong></p>
```

Podemos combinar estas etiquetas:

```html
<p>El siguiente texto va a estar en subrayado y en negrita:<u><b>Hola Mundo</b></u></p>
```

**ENLACE**

Esta etiqueta nos va a permitir navegar a páginas dentro de la aplicación o a enlaces externos como google…

 

```html
<a>Ir a la página de The Valley</a>
```

 

Tenemos que ponerle un atributo a la etiqueta diciendo a la página a la que queremos ir

```html
<a href="https://www.thevalley.es">Ir a la página de The Valley</a>
```

Este enlace se nos abre en la mima página, si queremos que se nos abra en otra pestaña tendremos que usar el atributo target

```html
<a href="https://www.thevalley.es" target="_blank">Ir a la página de The Valley</a>
```

**SALTOS DE LÍNEA**

La etiqueta ```<br> ```nos permite dar un salto de línea, por ejemplo, dentro de un párrafo. La etiqueta ```<br>``` no necesita cierre.

```html
<p>Este es mi contenido, <br>esto tiene que ir en otra línea</p>
```

**SEPARADOR DE CONTENIDO**

La etiqueta ```<hr>``` nos permite realizar una separación de contenido. Aparecerá una línea en nuestra web que hará la separación.

```html
<p>Este es mi primer contenido</p>
<hr>
<p>Este es mi segundo contenido</p>
```

**IMÁGENES**

La etiqueta ```<img>``` nos va a permitir introducir imágenes dentro de nuestra página web.

Al igual que otras etiquetas esta no tendría cierre. Sería necesario incluir el atributo src con la ruta de la imagen.

```html
<img src="imagen.jpg"> 
```

Dentro de esta etiqueta tenemos los atributos de **height** y **width** que nos van a permitir adaptar el tamaño de nuestra imagen. 

```html
<img src="imagen.jpg" width="100" height="200"> 
```

**LISTAS** 

La etiqueta ```<ul>``` nos permite crear un listado dentro de HTML, cada elemento de la lista estará identificado con la etiqueta ```<li>```. En caso de quere hacer una lista ordenada podemos usar <ol>

- Lista

```html
<p>Listado de películas Disney</p>
<ul>
  <li>Nemo</li>
  <li>Toy Story</li>
  <li>El rey león</li>
  <li>Mulan</l>
</ul>
```

- Lista ordenada

```html
<p>Ranking de mejores pelis de Disney</p>
<ol>
  <li>Toy Story</li>
  <li>El rey león</li>
  <li>Nemo</li>
  <li>Mulan</l>
</ol>
```

En las listas ordenadas podemos indicar con un atributo el número por el que queremos que empiece. De igual manera, podemos decir que haga una cuenta hacia atrás en vez de hacia delante

```html
<p>Ranking de mejores pelis de Disney</p>
<ol start="5" reversed>
  <li>Toy Story</li>
  <li>El rey león</li>
  <li>Nemo</li>
  <li>Mulan</l>
</ol>
```

Podemos también anidar listas:

```html
<ul>
  <li>Nemo</li>
  <li>
    Toy Story
    <ol>
      <li> Toy Story 1
        <ul>
          <li>Buddy</li>
          <li>Buzz</li>
          <li>Mr. Potato</li>
        </ul>
      </li>
      <li>Toy Story 2</li>
      <li>Toy Story 3</li>
      <li>Toy Story 4</li>
      <li>Lightyear</li>
    </ol>
  <li>El rey león</li>
  <li>Mulán</li>
</ul>
```

**TABLAS**

También podemos hacer tablas en HTML, para ello utilizaremos la etiqueta ```<table>```, para cada fila la etiqueta ```<tr>``` y para cada columna la etiqueta ```<td>```

Para que la tabla tenga aspecto visual de tabla podemos incluir dentro de la etiqueta table un atributo **border**

```html
<table border="1">
  <tr>
    <td>Manzanas</td>
    <td>3</td>
    <td>2€</td>
  </tr>
  <tr>
    <td>Peras</td>
    <td>6</td>
    <td>3,5€</td>
  </tr>
  <tr>
    <td>Melón</td>
    <td>1</td>
    <td>6€</td>
  </tr>
  <tr>
    <td>Naranjas</td>
    <td>6</td>
    <td>3€</td>
  </tr>
</table>
```

Para incluir la cabecera usaremos la etiqueta ```<th>```.

Para tablas grandes tenemos la estructura:

- ```<thead>``` para la cabecera
- ```<tbody>``` para el cuerpo de la tabla
- ```<tfoot>``` para el pie de la tabla

```html
<table border="1">
  <thead>
    <tr>
      <th>Frutas</th>
      <th>Unidades</th>
      <th>Precio</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Manzanas</td>
      <td>3</td>
      <td>2€</td>
    </tr>
    <tr>
      <td>Peras</td>
      <td>6</td>
      <td>3,5€</td>
    </tr>
    <tr>
      <td>Melón</td>
      <td>1</td>
      <td>6€</td>
    </tr>
    <tr>
      <td>Naranjas</td>
      <td>6</td>
      <td>3€</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td></td>
      <td>16</td>
      <td>14,5€</td>
    </tr>
  </tfoot>
</table>
```

**DIV**

La etiqueta ```<div>``` la utilizamos como un contenedor de bloque de contenido. Se usan para estructurar el contenido de la página web.

```html
<div>
  <h1>Noticia</h1>
  <p>Contenido de la noticia</p>

  <h1>Noticia 2</h1>
  <p>Contenido de la noticia</p>

  <h1>Noticia 3</h1>
  <p>Contenido de la noticia</p>
</div>

<div>
  <h1>Noticia deportiva 1</h1>
  <p>Contenido de la noticia</p>

  <h1>Noticia deportiva 2</h1>
  <p>Contenido de la noticia</p>

  <h1>Noticia deportiva 3</h1>
  <p>Contenido de la noticia</p>
</div>
```
