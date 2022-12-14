# DocumentaciónM4UF1

# GITHUB
Para crear un nuevo repositorio nos situamos en nuestro perfil en el apartado `Repositories` y clicamos en `New`.  
![Estilos](img/creaciongit2.png)

En el apartado de la creación podremos importar un repositorio con el codigo de otro clicando en `Import a repository` o crear uno de 0.  
Para crearlo agregaremos un nombre de repositorio, definiremos quien puede ver nuestro repositorio `Public o Private` y añadiremos un archivo readme clicando en la casilla `Add a README file` en caso de necesitarlo. Ahora simplemente le damos a `Create repository` y ya tendriamos el repositorio.
![Estilos](img/creaciongit3.png)

Una vez tengamos el repositorio acabado, lo subiremos a traves de Github pages.  
Para hacer esto tendremos que dirigirnos a la configuración `Settings`, luego al apartado `Pages` y seleccionar la rama que queramos subir, en este caso sera `main`.
La seleccionamos, guardamos clicando en `Save` y esperamos unos minutos.
![Estilos](img/creaciongit5.png)

En un par de minutos ya tendremos nustra pagina web subida.
![Estilos](img/creaciongit6.png)

Por último, si queremos trabajar con el repositorio en local, tendremos que dirigirnos a `Code` y copiar el HTTPS que luego pegaremos en local.
![Estilos](img/creaciongit4.png)


Para clonar un repositorio de Github en local copiaremos el codigo del repositorio y lo pegaremos en el terminal:  
![Estilos](img/git4.png)

Para subir los archivos a Github, tendremos que poner los siguientes comandos:

- Selecciona lo que queremos subir, en este caso ponemos `.` para seleccionar todo  
![Estilos](img/git1.png)

- Enviamos las actualizaciones que hemos hecho del repositorio `commit` y le damos un nombre a la version `-m`  
![Estilos](img/git2.png)

- Subimos el repositorio a Github  
![Estilos](img/git3.png)


# MARKDOWN

## Estilos de letra:
Para cambiar los estilos en Markdown usaremos asteriscos `*` y guiones bajos `_` 
Estos estilos se pueden combinar  

![Estilos](img/estilos.png)

*Cursiva*

**Negrita**

***Combinado***

## Encabezados:
Para crear encabezados en Markdown usamos las almohadillas `#`, añadiendo 1 por cada nivel hasta un maximo de 6.  
Puedes cerrar los encabezados añadiendo el mismo numero de almohadillas al final.  
Los encabezados tienen un estilo asociado por defecto.

 # #Encabezado 1
 ## ##Encabezado 2
 ### ###Encabezado 3
 #### ####Encabezado 4
 ##### #####Encabezado 5
 ###### ######Encabezado 6

## Parrafos y Saltos de linea:
Para generar un nuevo párrafo en Markdown simplemente separa el texto mediante una línea en blanco (pulsando dos veces intro)

Markdown no soporta dobles líneas en blanco, así que si intentas generarlas estas se convertirán en una sola al procesarse.  
Para realizar un salto de línea y empezar una frase en una línea siguiente dentro del mismo párrafo, tendrás que pulsar dos veces la barra espaciadora antes de pulsar una vez intro.


## Imagenes

### Imagen en linea  
Las imagenes en linea estan compuestas por una exclamación `!` para definir que estas haciendo una imagen, un texto alternativo `[]` y la dirección `()`:
`![TextoAlternativo](RutaImg.png)`

### Imagen de referencia  
Las imagenes de referenciaa estan compuestas por una exclamación `!` para definir que estas haciendo una imagen, un texto alternativo `[]` y la referencia `[]`.
Y donde queramos añadir la imagen pondremos el nombre de la referencia `[]` la dirección `:https//` y el texto alternativo `""`:
`![TextoAlternativo][NombreReferencia]
[NombreReferencia]:Link"TextoAlternativo"
`

## Enlaces
Los enlaces estan compuestos por el texto que contendra el link `[]`, el link `()`.  
`[Link](https://ejemplo.com/ "Título opcional del enlace")`  
[Link](https://google.com/)


## Listas:

### Listas ordenadas:
1. Para crear una lista ordenada usamos `numero.` Ej.: 1.
    1. Las listas se pueden anidar o combinar añadiendo 4 espacios antes del siguiente
5. El numero de la lista no es necesario que sea consecutivo ya que el numero cambia segun en la posición en la que se encuentre

### Listas desordenadas:
- Para crear una lista desordenada podemos usar: guion `-`, suma `+` o asterisco `*`
+ El simbolo usado para crear la lista no importa ya que todos se veran igual al procesarse
    * Estas listas tambien se pueden anidar o combinar


## Tablas
-Para crear las filas usaremos las barras verticles `|` entre una y otra
-Para crear un encabezado, debajo de este añadiremos una columna con las mismas filas separadas con `|` y en vez de texto, pondremos 2 o mas guiones `--`. En esta separación, podremos definir la alineación de las columnas con `:`
-Para añadir mas columnas simplemente seguiremos con la misma estructura (no hace falta que las columnas esten alineads verticalmente)

Ej:  
```
|Columna1|Columna2|Columna3|
|:--|--|--:|
|Texto1|Texto2|Texto3|
```
|Columna1|Columna2|Columna3|
|:--|--|--:|
|Texto1|Texto2|Texto3|


## Codigo
El codigo se tiene que introducir dentro de accentos graves '` `` `'.

`codigo`

Para crear un bloque que contenga codigo, este se ha de incluir entre tres accentos graves '` ``` `'.

```
codigo
```


# HTML
![HTML](img/HTML.png)


# CSS
CSS (Cascading Style Sheets) es un lenguaje de marcas que se utiliza para describir la apariencia de un documento escrito en HTML o XML dandoles estilo y formato, permitiendo cambiar el aspecto visual de un sitio web o aplicación.

## Ubicación
### Estilo en linea  
En el estilo en linea, el CSS se aplica directamente al elemento HTML mediante el elemento `style`. Por ejemplo:
```
<p style="color:red; font-size:20px;">Este párrafo tiene un estilo en línea</p>
```

### Estilo interno 
El estilo interno se añade a un elemento HTML mediante el elemento `style` en el encabezado del documento. Por ejemplo:
```
<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>
```

### Estilo externo 
Por último, el estilo externo se añade a un documento HTML mediante la etiqueta `link` en el encabezado del documento, y haciendo referencia a un archivo CSS externo. Por ejemplo:
```
<head>
  <link rel="stylesheet" type="text/css" href="estilos.css">
</head>
```
```
p {
  color: red;
  font-size: 20px;
}
```

## Estructura
La estructura que hay que seguir en los estilos internos y externos es la siguiente:
```
selector{
 atributo1;
 atributo2;
}
```

## Selectores
### Selector universal
El selector universal selecciona todos los elementos del documento. Se representa con el símbolo `*`. Por ejemplo, la siguiente regla CSS aplica un estilo a todos los elementos del documento:
```
* {
  color: red;
}
```

### Selector de id
El selector de ID selecciona un elemento con un determinado ID. Se representa con el símbolo `#` seguido del nombre del ID. Por ejemplo, la siguiente regla CSS selecciona el elemento con ID "título" y le aplica un estilo:
```
#titulo {
  font-size: 24px;
  font-weight: bold;
}
```

### Selector de clase
El selector de clase selecciona todos los elementos con una determinada clase. Se representa con el símbolo `.` seguido del nombre de la clase. Por ejemplo, la siguiente regla CSS selecciona todos los elementos con la clase "destacado" y les aplica un estilo:
```
.destacado {
  background-color: yellow;
}
```

### Selector de elemento
El selector de elemento selecciona todos los elementos de un tipo específico. Por ejemplo, la siguiente regla CSS selecciona todos los elementos "p"  y les aplica un estilo:
```
p {
  font-size: 16px;
}
```

### Selector de atributos
El selector de atributos selecciona elementos que tienen un determinado atributo o valor de atributo. Por ejemplo, la siguiente regla CSS selecciona todos los elementos "a" (enlaces) que tienen el atributo "href" con un valor que comience por "https":
```
a[href^="https"] {
  color: green;
}
```

### Selector de hijos
El selector de hijos selecciona elementos que son hijos directos de otro elemento. Se representa con el símbolo `>` entre dos selectores. Por ejemplo, la siguiente regla CSS selecciona todos los elementos "li" (elementos de lista) que son hijos directos de un elemento "ul" (lista sin ordenar):
```
ul > li {
  color: red;
}
```

### Selector de descendientes
El selector de descendientes selecciona elementos que están contenidos en otro elemento en el árbol de elementos del documento, independientemente de si son hijos directos o no. Por ejemplo, la siguiente regla CSS selecciona todos los elementos "li" (elementos de lista) que están contenidos en un elemento "ul" (lista sin ordenar), ya sea como hijos directos o como descendientes de algún otro elemento:
```
ul li {
  color: red;
}
```

### Selector de hermanos adyacentes
El selector de hermanos adyacentes selecciona elementos que están inmediatamente después de otro elemento en el árbol de elementos del documento. Se representa con el símbolo "+" entre dos selectores. Por ejemplo, la siguiente regla CSS selecciona todos los elementos "h2" que están inmediatamente después de un elemento "h1":
```
h1 + h2 {
  color: red;
}
```


## Pseudoclases
Las pseudoclases CSS son selectores que permiten aplicar estilos a elementos HTML en función de ciertos estados o condiciones específicas.
Las pseudoclases siempre empiezan por `:` por ejemplo `:hover` o `:focus`.


## Pseudoelementos
Los pseudoelementos CSS son selectores que permiten aplicar estilos a elementos específicos de un elemento HTML, como por ejemplo el primer o el último carácter de un párrafo.
Los pseudoelementos siempre empiezan por `::` por ejemplo `::before` o `::first-letter`.


## Atributos importantes
- MARGIN: El atributo margin es utilizado para establecer los márgenes externos de un elemento HTML. Ej: `margin: 20px;`.
- PADDING: El atributo padding es utilizado para establecer el relleno interno de un elemento HTML. Ej: `padding: 20px;`.
- TEXT-ALIGN: El atributo text-align es utilizado para alinear el texto de un elemento HTML. Ej: `text-align: center;`
- COLOR: El atributo color es utilizado para establecer el color del texto de un elemento HTML. Ej: `color: red`
- BORDER: El atributo border es utilizado para establecer un borde alrededor de un elemento HTML. El borde puede ser definido utilizando una combinación de propiedades. Ej: `border: 10px solid red;`
- BACKGROUND-COLOR: El atributo background-color es utilizado para establecer el color de fondo de un elemento HTML. Ej: `background-color: green;`
- WIDTH: El atributo width es utilizado para establecer el ancho de un elemento HTML. Ej: `width: 500px;`
- HEIGHT: El atributo height es utilizado para establecer la altura de un elemento HTML. Ej: `height: 300px;`
