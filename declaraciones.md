# :smiling_imp: declaraciones css

Una declaración de CSS es un bloque que especifica el conjunto de estilos que se añadirán a un elemento HTML, el cual esta estructurado por: 
<br>

* `selector`:  es el elemento o conjunto de elementos a los cuales se añadirán los estilos.
  
* `atributos o propiedades`: son los identificadores legibles que indican que caracteristicas de estilo se desea cambiar.
  
* `valores`:  indica cómo quieres que cambien esas características de estilo.

  <br>
  
  ## atributos para fuentes y textos

 ***
 ### color

 Este atributo sirve para definir el color del TEXTO de un elemento. Lo admiten casi todas las etiquetas HTML, ya que en casi todas podemos colocar texto. 
 Podemos colocar los colores con valores RGB, con nombres y otras anotaciones

 ~~~
h1 {
    color: blue;
}
.destacar {
    color: #ff3355;
}
 ~~~

 ### font-size

 Sirve para indicar el tamaño de las fuentes de manera exacta, permitiendo distintos tipos de unidades CSS, absolutas y relativas.
 Además, aunque no se usa mucho, existen como varios tamaños definidos por nombres, como xx-small, x-small, small, medium, large, x-large, xx-large, que dejan a juicio del navegador qué tamaño exacto usar.

~~~
footer {
    font-size: 1.25rem;
}
div .nota {
    font-size: small;
}
~~~

### font-family

Con este atributo indicamos la familia tipográfica que tendrán los elementos. Podemos indicar valores de fuentes específicas o algunos nombres de fuentes genéricos.

~~~
article {
    font-family: verdana;
}
p {
    font-family: serif;
}
~~~

Cuando usamos estos nombres genéricos el navegador es el que elige la fuente en particular que va a colocar. Será una familia tipográfica que respete el nombre genérico. Por ejemplo, si indicamos "sans-serif" el navegador podría elegir fuentes como arial, verdana, helvetica...
Estas fuentes genéricas se suelen usar como "fallback", de modo que, si no está la fuente que nosotros hemos definido anteriormente, usará cualquiera que se adapte al nombre genérico.

* `serif`
* `sans-serif`
* `cursive`
* `fantasy`
* `monospace`

 ~~~
span {
  font-family: 'Times New Roman', Times, serif;
}
 ~~~


### font-weight

Este atributo indica la espesura del texto, Se usa mucho para indicar que queremos un texto en negrita, pero también existen espesuras más finas que la normal, que son interesantes como recurso de diseño.
Podemos indicar la espesura con muchos tipos de valores. Los valores posibles son los siguientes:

Ten en cuenta que no siempre las fuentes que tienes instaladas soportan todas las espesuras. A veces descargamos una fuente que no tiene la espesura fina, o la negrita. En esos casos el navegador puede representar la fuente normal o hacer una aproximación de la espesura deseada de manera aproximada

* `normal` : Peso/grueso normal de la fuente. Igual que 400.
* `bold` : Grueso ancho (negrita). Igual que 700.
* `bolder` : Corresponde a un tipo de fuente más grueso que el tipo del elemento padre (dentro de los valores disponibles).
* `lighter` : Corresponde a un tipo de fuente menos grueso que el tipo del elemento padre (dentro de los valores disponibles).
* `100-500` : un valor entre 100 y 500 se presentará con el valor más próximo disponible para dar una letra más clara
* `600-900` : y entre 600 y 900, será bold.

~~~
b {
    font-weight: bolder;
}
h1 {
    font-weight: 300;
}
~~~

### font-style

Este atributo sirve para indicar si queremos fuente oblícua, es decir, itálica.
Los valores posibles son:

* `normal`
* `italic`
* `oblique`

Los valores "italic" o "oblique" son equivalentes.

~~~
li {
    font-style: italic;
}
~~~

<br>

## Atributos para bloques de texto

Antes hemos visto atributos "font", que permitían definir estilos para textos. Ahora vamos a ver estilos para el texto, lo que resulta bastante parecido. La diferencia de estos atributos es que a veces tienen sentido cuando se aplican sobre bloques de texto, como los párrafos.

### line-height

Este es un estilo fundamental para facilitar la lectura del texto. Sirve para definir la altura de las líneas del texto. Por tanto, podemos usarlo para especificar el espaciado entre líneas.

~~~
li {
    line-height: 24px;
}
body {
    line-height: 1.4em;
}
~~~

### text-decoration

Este atributo permite definir la decoración del texto, lo que equivale a si está subrayado o tachado, o por el contrario nada de eso.

valores posibles

* `none`
* `underline`
* `overline`
*  `line-trough`

 ~~~
a {
    text-decoration: none;
}
~~~

 ~~~
.tachado {
    text-decoration: line-through;
}
~~~
  
Un uso típico es quitarle el subrayado a los enlaces

### text-align

Este atributo sirve para indicar la alineación del texto. Es uno de esos atributos que solamente tiene sentido aplicar sobre bloques de texto, como los párrafos.

* `left`
*  `right`
*  `center`
*  `center`
*  `justify` : A veces justify no funciona en todos los sistemas. De todos modos, no es un estilo que se use mucho en la web, sino más bien en la maquetación de libros o revistas.

  
~~~
div.centrado {
    text-align: center;
}
.columna-numerica {
    text-align: right;
}
~~~

### text-indent

Este atributo permite establecer un sangrado o indentación (como un margen a la izquierda). No se suele usar mucho, la verdad, ya que es algo más típico de medios impresos.


~~~
p {
    text-indent: 16px;
}
~~~


### text-transform

Este atributo permite hacer transformaciones sobre el texto, que afectan al tamaño de caja (si son mayúsculas o minúsculas).

Es bastante útil como criterio de diseño. Los valores que podemos usar son estos:

* `uppercase` : todas en mayúsculas
* `capitalize` : la primera letra de cada palabra en mayúscula
* `lowercase` : todas en minúscula
* `none` : lo deja tal cual esté en el código HTML de la página


  ~~~
h3 {
    text-transform: uppercase;
}
  ~~~

link infrormacion https://desarrolloweb.com/articulos/186.php





 
  
