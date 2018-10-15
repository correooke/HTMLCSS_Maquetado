

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


