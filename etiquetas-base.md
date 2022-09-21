>[DIAPOSITIVAS](S2-recursos/etiquetas-base.pptx.pdf)

---

Vamos ahora a ver las etiquetas más importantes que pueden ayudarnos a formatear nuestro contenido.

Recordamos, una etiqueta tiene apertura, cierre y contenido. A su vez puede tener atributos.

``` html
<p style="color:blue;"> Párrafo de ejemplo <p>
```

Vamos primero aprender las etiquetas base que nos van a ayudar a estructura el código:

- ```<!DOCTYPE>``` Nos indica la versión de HTML
- ```<html>``` Raíz del archivo
- ```<head>``` Engloba la información adicional del documento que no va a ser visible
- ```<title>``` Título de la página. Ya lo hemos usado en nuestro “Hello World!”
- ```<link>``` Nos va a permitir conectar diferentes recursos externos como los archivos CSS
- ```<style>``` Nos permite incluir código CSS dentro del documento HMLT (No recomendado)
- ```<script>``` Permite incluir código JS o conectarlo con el documento HTML
- ```<meta>``` Permite incluir características a la página
- ```<body>``` Donde incluímos todo el contenido que queremos mostrar en HTML

TRUCO: Para crear una estructura html dentro de un fichero html en VSC podemos utilizar la abreviación  ```html:5```  o  ```!```  y pulsamos enter, el resultado es este:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

Nos quedaría por ver dentro del código la etiqueta ```<link>```, con la que hemos comentado que podemos conectar un archivo css

```html
<link rel="stylesheet" type="text/css" href="css/prueba.css">
```

La etiqueta ```<style> ``` con la que probamos a modificar el color de un título es la siguiente:

```html
<style type="text/css">
  h1 {
    color: yellow;
  }
</style>
```
