> [Solucion](S2-recursos/solucion-the-valley.zip)

---

Llega el momento de remangarnos, el equipo de The Valley nos ha pedido si podemos hacerles una página web con 3 másters nuevos que han sacado. Nos han enviado un pdf para mostrarnos como lo quieren:

> [Enunciado](S2-recursos/the-valley.pdf)

Revisando la documentación que nos han enviado vemos que tenemos una estructura similar a esta:

- Encabezado con una introducción (HEADER)
- Listado de navegación para acceder a los distintas secciones (NAV)
- Una sección con los diferentes másters (SECTION con ARTICLES)
- Una sección con el contenido de los másters (SECTION)
- Una sección de convocatorias y plazas (SECTION)
- Un pie de página. (FOOTER)

Tras crear nuestro proyecto en VSC, creamos una estructura básica HMTL y creamos una carpeta img con las imágenes que nos manda el equipo.

Creamos primero el header de la página que incluye la imagen (adaptamos el tamaño), el título y el slogan

```html
<header>
    <img height="100" src="img/img0.png"/>
    <h1>Másters digitales</h1>
    <p>Lidera el mundo profesional</p>
</header>
```

El segundo bloque que creamos es el menu navegación con un listado de secciones.

```html
<nav>
    <ul>
        <li>Conoce nuestros másters</li>
        <li>Contenido del máster</li>
        <li>Convocatorias y plazas </li>
    </ul>
</nav>
```

Vamos ahora a crear la sección de la descripción de los máster, cada uno de ellos estará encapsulado dentro de un article. ¿Qué etiquetas hemos usado?

- ```<h2>``` como título de la sección
- ```<hr>``` como separadores de contenido
- ```<img>``` para incluir la imagen de cada uno de los máster
- ```<p>``` para incluir los párrafos de contenido
- ```<i>``` para poner un contenido en cursiva
- ```<br>``` como salto de línea
- ```<strong>``` para enfatizar un contenido
- ```<u>``` para subrayar una parte del contenido

```html
<section>
    <h2> Conoce nuestros másters </h2>
    <hr>
    <article>
        <img height="300" src="img/img1.jpg" />
        <h3> Máster en Digital Product Management </h3>
        <p><i>Innova, lidera y hackea el crecimiento de productos digitales</i></p>
        <br>
        <p>
            El Product Manager es la clave para liderar la estrategia 
            de productos digitales: su concepción, desarrollo y crecimiento trabajando 
            con su equipo de desarrolladores, UX y Data para tomar las mejores 
            decisiones de producto.
        </p>
        <p>
            A través de esta experiencia formativa única articulada en torno a proyectos y retos 
            prácticos aprenderás a aplicar las metodologías y herramientas usadas por las startups tecnológicas 
            líderes para transformarte en un auténtico líder de productos digitales.
        </p>
        <p>
            <strong><u>Posiciones profesionales relacionadas:</u></strong> Product Manager, Product Designer, Consultor de negocio.
        </p>
        <hr>
    </article>
    <article>
        <img height="300" src="img/img2.jpg" />
        <h3> Desarrollo Web: Front End</h3>
        <p><i>Innova, lidera y hackea el crecimiento de productos digitales</i></p>
        <br>
        <p>
            100% enfocado a la empleabilidad: 6 semanas dedicadas a practicar intensamente desarrollando 3 proyectos, con un proyecto final real 
            sponsorizado por una empresa, y co-creado con empresas tecnológicas.
        </p>
        <p><strong><u>Posiciones profesionales relacionadas:</u></strong> Desarrollador Web, Desarrollador Front-end, Desarrollador de React.</p>
        <hr>
    </article>
    <article>
        <img height="300" src="img/img3.jpg" />
        <h3> Impact MBA</h3>
        <p><i>Fórmate para ser parte activa del cambio de eras</i></p>
        <br>
        <p>
            Conviértete en un profesional flexible, capacitado para adaptarse al cambio gracias al desarrollo de conocimientos, competencias y 
            herramientas que las empresas reclaman. Con foco en las posibilidades que las tecnologías disruptivas ofrecen y su aplicación en el mundo 
            de los negocios, buscando siempre el impacto positivo en la sociedad. Desarrollarás una orientación humanista y ética, dirigida a una realidad 
            cada vez más tecnologizada para ser capaz de emprender un proyecto desde el día inicio y hacerlo realidad..
        </p>
        <p><strong><u>Posiciones profesionales relacionadas:</u></strong> Jefe de proyecto, PMO...</p>
        <hr>
    </article>
</section>
```

Tras la sección de másters vamos a hacer la sección de ‘Contenidos del máster’ cuya principal dificultad son las listas anidadas:

```html
<section>
	<h2> Contenido de los Másters </h2>
	<hr>
	<ul>
	    <li>
	        Máster en Digital Product Management
                <ol>
	            <li>Lean Business Design & Innovation</li>
	            <li>Product Management & Strategy</li>
	            <li>Product Growth</li>
	        </ol>
	    </li>
	    <li>
	        Desarrollo Web: Front End
		<ol>
	            <li>Prework</li>
	            <li>Fundamentos web & JS</li>
	            <li>Desarrollo web Front-end</li>
	            <li>Desarrollo web Back-end</li>
	        </ol> 
	    </li>
	    <li>
	        Impact MBA
	        <ol>
	            <li>Conoce los grandes ámbitos de la disrupción a través de las nuevas tecnologías</li>
	            <li>Idea y prototipa productos innovadores</li>
	            <li>Aprende a hacer un Business Plan</li>
	            <li>Haz crecer tu negocio a través del marketing</li>
	        </ol>
	    </li>
	</ul>
	<hr>
</section>
```

Le llega el turno a la sección ‘Convocatorias y Plazas’ la cual incluye una tabla dentro de su contenido con las plazas disponibles y las próximas convocatorias:

```html
<section>
    <h2> Convocatorias y plazas </h2>
    <hr>
    <br>
    <table border="1">
        <thead>
            <tr>
                <th>Máster</th>
                <th>Próxima convocatoria</th>
                <th>Plazas disponibles</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Máster en Digital Product Management</td>
                <td>Octubre 2022</td>
                <td>13 plazas disponibles</td>
            </tr>
            <tr>
                <td>Desarrollo Web: Front End</td>
                <td>Noviembre 2022</td>
                <td>2 plazas disponibles</td>
            </tr>
            <tr>
                <td>Impact MBA</td>
                <td>Abril 2023</td>
                <td>15 plazas disponibles</td>
            </tr>
        </thead>
    </table>
    <br>
</section>
```

Por último el footer, con el copyright:

```html
<footer>
    <hr>
    <p>© 2022 The Valley Digital Business School. Developed by <b>Edu</b></p>
    <hr>
</footer>
```

¡¡PLUS!! Vamos ha hacer que el menú de navegación sea utilizable y nos lleve a las diferentes secciones, para ello utilizaremos la etiqueta ```<a>``` dentro del menú de navegación.

Tenemos que indicarle a dónde navegamos, esto va a ser a las diferentes secciones. Cada una de ellas tiene que tener un atributo único que las identifique, por lo que utilizamos id.

```html
<section id="seccion1">
```

Desde nuestro enlace referenciaremos ese id dentro de la etiqueta href con un # indicando que nos lleve a la etiqueta con es id.

```html
<ul>
		<li><a href="#seccion1">Conoce nuestros máster</a></li>
		<li><a href="#seccion2">Contenido del máster</a></li>
		<li><a href="#seccion3">Convocatorias y plazas</a></li>
</ul>
```

Ya habríamos terminado nuestra página web, el resultado final:

[ Si copias y pegas este código, acuérdate de meter en el proyecto las imágenes dentro de la carpeta img, las tienes en el fichero que te adjuntamos ]

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cursos The Valley</title>
</head>
<body>
    <header>
        <img height="100" src="img/img0.png"/>
        <h1>Másters digitales</h1>
        <p>Lidera el mundo profesional</p>
        <hr>
    </header>
    <nav>
        <ul>
            <li><a href="#seccion1">Conoce nuestros máster</a></li>
            <li><a href="#seccion2">Contenido del máster</a></li>
            <li><a href="#seccion3">Convocatorias y plazas</a></li>
        </ul>
        <hr>
    </nav>
    <main>
        <section id="seccion1">
            <h2>Conoce nuestros másters</h2>
            <hr>
            <article>
                <img height="300" src="img/img1.jpg" />
                <h3>Máster en Digital Product Management</h3>
                <p><i>Innova, lidera y hackea el crecimiento de productos digitales</i></p>
                <br>
                <p>
                    El Product Manager es la clave para liderar la estrategia de productos digitales: 
                    su concepción, desarrollo y crecimiento trabajando con su equipo de desarrolladores, UX y Data 
                    para tomar las mejores decisiones de producto.
                </p>
                <p>
                    A través de esta experiencia formativa única articulada en torno a proyectos y retos prácticos
                    aprenderás a aplicar las metodologías y herramientas usadas por las startups tecnológicas líderes 
                    para transformarte en un auténtico líder de productos digitales.
                </p>
                <p>
                    <b><u>Posiciones profesionales relacionadas:</u></b> Product Manager, Product Designer, Consultor de negocio.
                </p>
                <hr>
            </article>
            <article>
                <img src="img/img2.jpg" height="300" />
                <h3>Desarrollo Web: Front End</h3>
                <p><i>Innova, lidera y hackea el crecimiento de productos digitales</i></p>
                <br>
                <p>
                    100% enfocado a la empleabilidad: 6 semanas dedicadas a practicar intensamente desarrollando 3 proyectos, 
                    con un proyecto final real sponsorizado por una empresa, y co-creado con empresas tecnológicas.
                </p>
                <p>
                    <b><u>Posiciones profesionales relacionadas:</u></b> Desarrollador Web, Desarrollador Front-end, Desarrollador de React.
                </p>
                <hr>
            </article>
            <article>
                <img src="img/img3.jpg" height="300" />
                <h3>Impact MBA</h3>
                <p><i>Fórmate para ser parte activa del cambio de eras</i></p>
                <br>
                <p>
                    Conviértete en un profesional flexible, capacitado para adaptarse al cambio gracias al desarrollo de conocimientos, competencias 
                    y herramientas que las empresas reclaman. Con foco en las posibilidades que las tecnologías disruptivas ofrecen y su aplicación 
                    en el mundo de los negocios, buscando siempre el impacto positivo en la sociedad. Desarrollarás una orientación humanista y ética, dirigida a una realidad cada vez más tecnologizada para ser capaz de emprender un proyecto desde el día inicio y hacerlo realidad..
                </p>
                <p>
                    <b><u>Posiciones profesionales relacionadas:</u></b> Jefe de proyecto, PMO...
                </p>
                <hr>
            </article>
        </section>
        <section id="seccion2">
            <h2>Contenido del máster</h2>
            <hr>
            <ul>
                <li>
                    Máster en Digital Product Management
                    <ol>
                        <li>Lean Business Design & Innovation</li>
                        <li>Product Management & Strategy</li>
                        <li>Product Growth</li>
                    </ol>
                </li>
                <li>
                    Desarrollo Web: Front End
                    <ol>
			<li>Prework</li>
                        <li>Fundamentos web & JS</li>
                        <li>Desarrollo web Front-end</li>
                        <li>Desarrollo web Back-end</li>
                    </ol>
                </li>
                <li>
		    Impact MBA
                    <ol>
                        <li>Conoce los grandes ámbitos de la disrupción a través de las nuevas tecnologías</li>
                        <li>Idea y prototipa productos innovadores</li>
                        <li>Aprende a hacer un Business Plan</li>
                        <li>Haz crecer tu negocio a través del marketing</li>
                    </ol>
                </li>
            </ul>
            <hr>
        </section>
        <section id="seccion3">
            <h2>Convocatorias y plazas</h2>
            <hr>
            <br>
            <table border="1">
                <thead>
                    <tr>
                        <th>Másters</th>
                        <th>Próxima convocatoria</th>
                        <th>Plazas disponibles</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Máster en Digital Product Management</td>
                        <td>Octubre 2022</td>
                        <td>13 plazas disponibles</td>
                    </tr>
                    <tr>
                        <td>Desarrollo Web: Front End</td>
                        <td>Noviembre 2022</td>
                        <td>2 plazas disponibles</td>
                    </tr>
                    <tr>
                        <td>Impact MBA</td>
                        <td>Abril 2023</td>
                        <td>15 plazas disponibles</td>
                    </tr>
                </tbody>
            </table>
            <br>
            <hr>
        </section>
    </main>
    <footer>
        <p>© 2022 The Valley Digital Business School. Developed by <b>Edu</b></p>
        <hr>
    </footer>
</body>
</html>
```
