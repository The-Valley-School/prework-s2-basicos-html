¡Vamos a hacer ya nuestro primer web en html! Para ello tenemos que abrir Visual Studio Code y seguir los siguientes pasos:

- Abrimos VSC que tenemos descargado
- Pulsamos el botón explorador y seleccionamos la carpeta donde queremos guardar nuestro proyecto
- Pulsamos en crear un nuevo archivo y lo llamamos **index.html** . La raíz de una página web siempre va a ser index.html
- Vamos a la carpeta del proyecto y vemos que está este nuevo archivo, al pulsarlo nos abrirá el navegador con una pantalla en blanco, este va a ser nuestra primera web. Volvemos a VSC para trabajar sobre ella

Lo primero que tenemos que hacer es crear nuestra estructura html:

```html
<!DOCTYPE html>
<html>
    <head>
        
    </head>
    <body>
        
    </body>
</html>
```

Vamos ahora a mostrar nuestra primera frase en el navegador, vamos a utilizar la etiqueta título **h1**  para ello:

```html
<h1> Hello World! </h1>
```

Guardamos, recargamos la pestaña del navegador ¡ya nos muestra el mensaje!

Para ponerle el lazo a este primer proyecto, vamos a cambiar el título de la pestaña que aparece en el navegador, para ello introducimos dentro del <head> la siguiente información:

```html
<title> Mi primer ejercicio </title>
```

Con esto ya tendríamos nuestro primer proyecto web, el código completo quedaría así:

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Mi primer ejercicio</title>
    </head>
    <body>
        <h1>Hello World!</h1>
    </body>
</html>
```
