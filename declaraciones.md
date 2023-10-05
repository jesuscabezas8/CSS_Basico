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


 
  
