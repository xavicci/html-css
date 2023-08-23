Es un sistema de columnas creado por nosotros de acuerdo a las necesidades para ajustar nuestros elementos y componentes.
La mejor herramienta de CSS para crear una grilla es Grid.
Sass es un pre-procesador de CSS te ayuda a escribir CSS de una manera más rápida y más fácil.
Mixin es una clase que tiene dentro del pre-procesador, que te ayuda a manejar mejor los Breakpoints.
Tenemos que configurar nuestros BreakPoints (Tipos de pantalla).
• $xs: 360px. Para móviles pequeños.
• $s: 440px. Para móviles con la pantalla más grande.
• $m: 768px. Para tablets.
• $l: 1280px. Para Ordenadores pantalla normal.
• $xl: 1440px. Monitores de alta calidad.

Podemos usar un Mixin para manejar los distintos breakpoints más fácilmente.
Después vamos a configurar nuestras variables dependiendo de los breakpoints.
–columns. Es el número de columnas que vamos a poner.
–column-gap es el espacio entre las columnas.
Creamos después una clase Grid para configurar cada uno de los elementos contenedores donde vamos a incluir nuestros componentes.

Para aquellos que se pregunten porque se usa una cuadricula de 12 columnas, la razón es que el 12 es el mínimo común múltiplo optimo por englobar la mayor cantidad de números sin ser excesivamente grande.
De esta forma se pueden crear 2, 3, 4, 6 ó 12 columnas del mismo tamaño sin recurrir a fracciones.