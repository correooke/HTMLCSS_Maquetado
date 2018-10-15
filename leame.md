

#2

agregamos el contenedor principal "main" y el contenedor del pie "footer"
en el css agregamos selector de id que lleva el simbolo numeral o hash seguido del nombre del identificador del elemento. Vamos a utilizar el alto con vh que nos refiere a la altura del viewport (que sería view height), donde 100 vh será equivalente al alto total de la pantalla. 


El ancho lo establecemos a 100vw, para los dos elementos. 

También vamos a utilizar background-color para establecer el color de fondo de cada contenedor. El primero vamos a utilizar un color con nombre "orange", y el segundo vamos a utilizar la función rgb. 

#3

Ahora tenemos el contenedor principal y el pie que se ajustan de manera proporcional, lo que en realidad no es un efecto deseado. 
Para lograr que el pie tenga un tamaño fijo vamos a utilizar la unidad de medida "pixeles". Para que el contenedor principal ocupe el espacio restante de la pantalla vamos a utilizar la función de CSS3 "calc". Esta función nos permite realizar cálculos y mezclar diferentes tipos de unidades. Es una función bastante nueva, pero ya es soportada por todos los navegadores actuales.   
Utilizando calc y restando el alto que le vamos a otorgar al pie, que va a ser de 50 pixeles, vamos a darle tamaño al contenedor principal. 

Importante: 
las operaciones + y - siempre deben de estar separados de sus operandos mediante espacios en blanco

https://developer.mozilla.org/es/docs/Web/CSS/calc

#4 

Al contenedor principal le definimos un ancho máximo para que cuando la pantalla tenga un ancho mayor a 400 pixeles los elementos que tenemos en nuestra página no se exparsan ni ocupen más espacio del que queremos. Tambien utilizamos el margin auto, para que este bloque quede centrado. 

Vamos a definir también un ancho y un alto mínimo, así no se "rompe" el diseño si el usuario achica demasiado la pantalla o se ve en un teléfono con pantalla pequeña. Una vez que se achique a un tamaño inferior a 520 px de alto, o 320 px de ancho, van a aparecer las barras de scroll. 

#5

Vamos a ver cómo agregar un texto en el pie de pagina, centrarlo y aplicarle un estilo de fuente.
Primero agregamos el elemento "p", principalmente utilizado para párrafos, y escribimos el texto que estaba definido en el diseño. 
Luego en el css vamos a asignar un color de fuente al selector del elemento contenedor principal, así todo el texto que ubiquemos dentro de este contenedor adquiere ese color por defecto. En este caso vamos a utilizar un color con nombre, con una palabra clave que representa al color blanco. 

Luego para que el texto quede centrado horizontalmente vamos a utilizar "text-align" center. 

Al texto podemos cambiarle el tamaño y la tipografía, mediante la propiedad "font". Primero definimos el tamaño en 14 pixeles, (tambien se suele utilizar la medida em) y seguido, definimos el tipo de fuente a Helvetica. Si el navegador no tuviera ese tipo de fuente, definimos una fuente por defecto genérica, "sans-serif".
Por último, le vamos a establecer el grosor de la fuente en bold, esto se hacer mediante la propiedad font-weight.

https://developer.mozilla.org/en-US/docs/Web/HTML/Applying_color

#6 

Vamos a centrar el texto del footer en la vertical. Para eso vamos a utilizar un tipo de selector CSS que nos permite hacer referencia a elementos que se encuentran dentro de un elemento contenedor. En este caso vamos a hacer referencia a todos los elementos del tipo "p" que esten dentro del elemento identificado como "footer-cont". Para el caso, tenemos un único elemento, pero podrían ser varios, y este selector estaría afectando a todos los que existiesen. 
Vamos a establecer el alto de línea con la propiedad "line-height", y vamos a igualar este alto al alto del contenedor. Por eso le asignamos el valor de 50 pixeles. 


