# 👣 Paso 2- Maquetado básico de la página
En este paso vamos a crear el maquetado básido de nuestra página. Esto significa separar la pantalla de manera tal que el contneido se muestre según nuestro diseño.
Lo que deberían obtener es lo siguiente:

![layout_result](https://github.com/german-egg/carrer-frontend/assets/90975517/5e38b23c-b24d-4d26-bdb1-8edc2a5559a5)

Para lograr esto vamos a seguir los siguientes pasos:

**1. Estructura del documento.**

Abrimos el proyecto creado en el paso anterior y en el archivo index.html, dentro de las etiquetas body (es decir, `<body> {etiquetas a agregar} </body>`) agregamos las siguientes etiquetas:
   * `<header></header>`
   * `<section></section>`
   * `<article></article>`
   * `<footer></footer>`

```html
<body>
    <header></header>
    <section></section>
    <article></article>
    <footer></footer>
</body>
```
Lo que acabas de escribir es la estructura principal de nuestro layout donde las etiquetas agregadas son “hijos” del contenedor principal (body). Esto se llama anidación en html.

La anidación en HTML se refiere a la práctica de colocar un elemento HTML dentro de otro elemento HTML. El elemento que se coloca dentro de otro se conoce como "elemento hijo" o "elemento anidado", mientras que el elemento que contiene al otro se llama "elemento padre" o "elemento contenedor".


**2. Atributos HTML.**

Los atributos HTML son información adicional que puedes añadir a las etiquetas para configurar o personalizar su comportamiento. Por ejemplo, en un enlace (<header>), el atributo class especifica la clase css que aplica a este contenedor. Los atributos generalmente aparecen dentro de la etiqueta de apertura y se escriben como pares nombre=”valor”.

```html
<header class="header"></header>
```
Para comenzar a aplicar estilos css a nuestro layout, debemos agregar un atributo de clase a algunos de nuestros elementos. Comencemos con cada etiqueta agregandole una clase que la defina. 

```html
<body>
    <header class="header"></header>
    <section class="hero"></section>
    <article class="main"></article>
    <footer class="footer"></footer>
</body>
```
4. **Estilos**

Para agregar estilos a nuestra card, primero debemos escribir una etiqueta <style></style> dentro de nuestro archivo html, justo antes de la etiqueta de cierre </head>. 
Dentro de esta etiqueta es donde podremos seleccionar los elementos HTML a los cuales les definimos atributos para modificar sus estilos. 

Un selector CSS es como un "etiquetador" que usas para decirle al navegador a qué elementos HTML quieres aplicar ciertos estilos. Por ejemplo, si quieres que todos los elementos con clase  (.class) de tu página tenga un ancho determinado, usas el selector .card en tu bloque de estilos para hacerlo:

```html
<head>
...
  <style>
   .header{
        width: 790px;
    }
  </style>
</head>

```

Terminemos de aplicar las propiedades necesarias a nuestro layout.

```html
<style>
  .header {
    background-color: #FF967F;
  }
  .hero {
    background-color: #476189;
  }
  .main {
    background-color: #D9D9D9;
  }
  .footer {
    background-color: #F6FFBB;
  }
</style>
```

Una propiedad CSS es un tipo de instrucción que se utiliza para definir cómo debe verse o comportarse un elemento HTML. Se coloca dentro de un bloque de código CSS, que está encerrado entre llaves { } y se asocia con un selector. Cada propiedad css tiene un nombre y un valor separados por “:”. Cada propiedad css finaliza con “;”

* width: 790px;
Establece el ancho del elemento en 790 píxeles.
* background-color: linear-gradient(180deg, #E4BFE8 0%, #93FCAA 100%);
Crea un fondo degradado que comienza con el color #E4BFE8 y termina con el color #93FCAA, yendo de arriba a abajo (180 grados).
text-align: center;
Centra horizontalmente el texto dentro del elemento.
padding: 41px 175px;
Añade un relleno alrededor del contenido del elemento, con 41 píxeles en la parte superior e inferior y 175 píxeles en los lados izquierdo y derecho.
border-radius: 15px;
Redondea las esquinas del elemento con un radio de 15 píxeles.

📌 Los valores del tipo #E4BFE8 son un código de color en formato hexadecimal utilizado en CSS para especificar un color particular. En este sistema, los colores se representan con seis dígitos hexadecimales pero CSS también nos permite declarar algunos colores comunes con sus nombres en inglés como “red”, “black”, “white” etc.







































































