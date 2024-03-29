# ASIX1 M4 APUNTES

Aqui iré escribiendo los apuntes de la asignatura M4 

## Primer Capitulo: MARKDOWN

Como poner el texto en *cursiva*?

```
*texto* o _texto_
```

Como poner el texto en **Negrita?**

```
**Texto** o __Texto__
```

Como Juntar ***las dos?***

```
Hay varias maneras, pero basicamente es alterar entre los dos, por ej:
_**texto**_ o __*texto*__...

```

Como Crear

* Una
* Lista
* Sin Enumerar?

```
* Lista (qualquier palabra)
* Texto
* Texto
o
+ Lista (qualquier palabra)
+ Texto
+ Texto
y asi...
```

Como crear una

1. lista
2. ordenada?

```
1. 1r paso
2. 2ndo paso
```

Como se ~~Tacha~~ el texto?

```
~~Texto~~
```

| Como  | Hacer | Una |
|--------|:---------:|---------:|
| Tabla | Como | Esta? |

Las lineas del medio ayudan a formatear la tabla, si solo pones guiones se orienta a la derecha, si lo cierras entre dos puntos, estará centrado, si pones solo a la derecha, se pondra a la derecha

Importante mencionar que si pones varias filas, va cambiando de color (cebra style) y la primera fila, se pondra como encabezado y se pondra el texto en negrita

```
Para crear una tabla, solo hay que escribir asi
| Titulo 1 | Titulo 2 | Titulo 3 |
|--------|:---------:|---------:|
| Texto 1 | Texto 2 | Texto 3 |
```

Como crear submenús?

* Primera opción de Lista Desordenada
* Segunda opción de Lista Desordenada
* Tercera opción de Lista Desordenada
    1. Primer submenú
    2. Segundo submenú

```
* Primera opción de Lista
* Segunda opción de Lista 
* Tercera opción de Lista 
    1. Primer submenú
    2. Segundo submenú
```

Inicio de un documento HTML

```
<html>
<head>
    <title>Titulo de documento</title>
</head>
<body>
    <p>Esto es un parrafo</p>
</body>
</html>
```

Como añadir un [*Enlace?*](https://github.com/JoelBarrantess "Enlace a mi user de github")

```
[Texto](URL "Texto cuando pones el mouse por encima")
```

Como añadir una *Imagen* como esta?

![Imagen](imagen.png "Imagen de teemo")

```
 ![Texto opcional](Imagen.png "Texto pasar mouse por encima")
```


[ ] Opción A

[X] Opción B

[ ] Opción C

No se formatea esto :(


## Segundo Capitulo: HTML

Se refiere a (Hypertext Markup Language), es un lenguaje de marcas, no es de programación solo renderiza etiquetas

#### Como funciona HTML?

Las etiquetas tienen que tener apertura y cierre, como en el ejemplo de abajo

```
<p> Conetenido </p>
```

Podemos modificar el comportamiento de una etiqueta para que se vea diferente, como una clase, que nos ayuda a la hora de clasificarlos

```
<p class="Valor"> Conetenido </p>
```

Se pueden anidar etiquetas (añadir etiquetas dentro de otras), por ejemplo como poner texto en negrita

```
<p> <strong> Conetenido </strong> </p>
```

#### Etiqueta IMG

La etiqueta IMG sirve para introducir imagenes, funciona con "href"

```
<img href="./imagen.png"></img> 
```

#### Como separar lineas

Se hace simplemente con la etiqueta `<br>`, no se cierra, es de un solo uso

```
<br>
```
También tenemos la etiqueta `<hr>`, que es lo mismo, pero con una linea que los separa

```
<hr>
```

#### Como crear un documento HTML

Primero una vez ya tenemos el documento creado, hay varias etiquetas, pero escribiendo "!" o "html:5", nos escribira el inicio del documento solo

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ayuda</title>
</head>
<body>
    
</body>
</html>
```

#### Etiquetas HTML

Un documento HTML siempre tiene que empezar por `<!Doctype HTML>` ya que perimte que se renderize en todos los navegadores, en la siguiente linea, escogemos el idioma de HTML, en nuestro caso, usamos ingles ("en").

Luego, tenemos la etiqueta `<Head>`, aqui se determinan todo lo no visible para el usuario en la pagina web
Aque dentro entran los metadatos por ejemplo, en la cuarta linea podemos ver el charset y el viewport.

Además, tenemos la etiqueta `<Title>`, la cual indica el titulo del documento arriba en las pestañas, se le podria añadir un icono con la etiqueta `<favicon>`

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ayuda</title>
</head>
```

Dentro de la etiqueta `<body>`, va todo el documento

```
<body>
</body>
```

Como hacer una lista?

Lista ordenada (Etiqueta `<ol>`)
```
<ol>
    <li>Primer elemento</li>
    <li>segundo elemento</li>
    <li>Tercer elemento</li>
</ol>
```
Lista desordenada (Etiqueta `<ul>`)
```
<ul>
    <li>Primer elemento</li>
    <li>segundo elemento</li>
    <li>Tercer elemento</li>
</ul>
```
Como poner un enlace?
```
<a href="https://www.google.com" alt="Por aqui se va a google" target="_blank">Esto es un enlace a google</a>
```
El alt sirve para mostrar texto cuando tienes el raton encima y target dice en este caso que se abre en otra pagina

Y para poner una cita es con la etiqueta `<blockquote>`
```
<blockquote>Esto es una cita</blockquote>
```

Para intoducir comentarios es con `<!-- comentario -->`
```
<!-- Esto es un comentario -->
```

Las rutas absolutas son las rutas empezando desde la raiz y las rutas relativas es de las que empiezan desde algún lado

![Imagen](https://i.ytimg.com/vi/h3EmdNFnRac/maxresdefault.jpg "imagen sobre las rutas")

Como se hace una tabla en HTML?

Con la etiqueta `<Table>`, `<Thead>`, `tbody` y `<Tfoot>`

Las rows con `tr` y las columnas 

```
<table border="1">
        <thead>
            <tr>
                <th>Puesto</th>
                <th>Atleta</th>
                <th>Tiempo</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1r</td>
                <td>Juan</td>
                <td>2:00</td>
            </tr>
            <tr>
                <td>2rd</td>
                <td>Juan</td>
                <td>3:00</td>
            </tr>
            <tr>
                <td>3th</td>
                <td>Pepe</td>
                <td>4:00</td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <th>Puesto</th>
                <th>Atleta</th>
                <th>Tiempo</th>
            </tr>
        </tfoot>
    </table>
```


#### Divs en HTML

un div sirve para distribuir y organizar el codigo html en general, tambien ayuda para clasificarlos en contenedores que pueden englobar una clase o un ID y asi ayuda a hacer el css y el html mas simple de entender para una persona

```
<div>
    <p>contendio del div </p>
</div>
```


## Tercer Capitulo: CSS

Hay tres maneras de aplicar el cocigo CSS en HTML

1. en la propia etiqueta (Inline)

2. En el head (Inserción interna)

3. En un archivo externo enlazado con la pagina (Inserción externa)

Para linkear la pagina al css se usa la etiqueta link

```
<link rel="stylesheet" href="./css/style.css" type="text/css">
```

## Selectores CSS
En css hay diferentes tipos de selectores:

#### Selector de tipo
Selecciona todos los elementos de un tipo específico.
```
p {
    color: blue;
}
```
Este ejemplo selecciona todos los elementos <p> y les asigna un color azul.

#### Selector de clase
Selecciona elementos que tienen un atributo de clase específico.
```
.destacado {
    font-weight: bold;
}
```
Este selector selecciona todos los elementos con la clase "destacado" y les aplica negrita.

#### Selector de ID
Selecciona un elemento con un ID específico.
```
#encabezado {
    background-color: gray;
}
```
Este selector selecciona el elemento con el ID "encabezado" y le asigna un color de fondo gris.

#### Selector universal
Selecciona todos los elementos en la página.
```
* {
    margin: 0;
    padding: 0;
}
```
Este selector selecciona todos los elementos y establece los márgenes y el relleno a cero.

#### Selector descendente
Selecciona un elemento que es descendiente de otro.
```
article p {
    color: green;
}
```
Este selector selecciona todos los elementos `<p>` que son descendientes de un elemento `<article>` y les asigna un color verde.


## Flex Responsive

Con un diseño responsive en una pagina web, se puede conseguir que cambie todo sobre la pagina en el momento que el tamaño de la pantalla es diferente, para hacer esto, se usa el `@media`

```
.columna {
    flex: 1;
    /* Inicialmente, cada columna ocupa el 33% del ancho disponible */
    width: 33.33%;
}

/* @media query para pantallas más pequeñas */
@media (max-width: 600px) {
    .columna {
        /* En pantallas más pequeñas, las columnas ocupan el 100% del ancho */
        width: 100%;
    }
}
```