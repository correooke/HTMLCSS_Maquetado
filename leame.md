

#2

agregamos el contenedor principal "main" y el contenedor del pie "footer"
en el css agregamos selector de id que lleva el simbolo numeral o hash seguido del nombre del identificador del elemento. Vamos a utilizar el alto con vh que nos refiere a la altura del viewport (que sería view height), donde 100 vh será equivalente al alto total de la pantalla. 

https://developer.mozilla.org/es/docs/Web/CSS/calc

Utilizando calc y restando el alto que le vamos a otorgar al pie, que va a ser de 50 pixeles
El ancho lo establecemos a 100vw, para los dos elementos. 

También vamos a utilizar background-color para establecer el color de fondo de cada contenedor. El primero vamos a utilizar un color con nombre "orange", y el segundo vamos a utilizar la función rgb. 
