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





 
  
