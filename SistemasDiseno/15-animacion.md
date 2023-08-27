https://www.youtube.com/watch?v=uDqjIdI4bF4


Si bien, los sistemas de diseño han sido trabajados arduamente para encaminar tanto el diseño mismo como al código, lo requerimientos con respecto al movimiento falla rotundamente debido a la repetibilidad, ahorro de tiempo y consistencia de UX.
.

ℹ️ Definición
El movimiento es una cualidad de un sistema de diseño que expresa atención visual, educación evocativa y centramiento visual.

.
Para otorgar movimiento a un sistema de diseño, se contemplan los siguientes pasos:
.

Conoce a tu audiencia
✨ Concepto clave
Antes de crear algo nuevo, cerciórate de aquello que ya exista.

.
Recuerda que en la misma medida que encaminas tus patrones de UI, es posible guiar los patrones de movimiento.
.
Al mencionar patrones de movimiento, nos referimos a:

Curvas de tiempo (Timing curves)
Tipos de uso como expresión, focalización e información
Coreografía (número de objetos en escena)
Efectos como escala opacidad, elevación
Movimiento vs estático
Sobremovimiento
.
image

Tabla de patrones

.

Creación de principios
✨ Concepto clave
La adoctrinación de cuándo y cómo usar el movimiento puede amenazar la consistencia del producto.

.
Para encontrar el equilibrio adecuado, se puede tomar como contexto a aquellas mejoras sobre UX:

¿Dónde necesitamos mayor acción e intención?
¿Dónde se puede desorientar los usuarios dentro de nuestra navegación?
.
Por ejemplo, tomando como referencia las guías de Material Design del cual define 3 principios de movimiento:

Informativo
El movimiento informa a los usuario de aquellas relaciones entre elementos o disponibilidad de ación.
.
Focalizado
El movimiento focaliza la atención sobre aquello importante sin generar distracción.
.
Expresivo
El movimiento celebra momentos en el uso del usuario al agregarle símbolos a interacciones comunes, expresando la personalidad de la marca.
.
Encuadre de construcción
✨ Concepto clave
El movimiento como pieza de animación dentro de un sistema de diseño es una relación enter un objeto, su tiempo y efecto.

.
Con los principios establecidos como equipo, el encuadre de movimiento consiste de una duración, ease, efectos (estado inicial y final) y coreografía.
.

ℹ️ Definición
Una duración describe una relación en temporalidad que modifica, por efecto, a un objeto.

.
En concepto de escalas, la duración puede ser vista en medidas como la tipografía, grilla e incluso color.
.
image

Así como la tipografía posee escalas en función de etiquetas (h1 … h6), es posible etiquetar a la duración como (t1 … t6) o mediante descripción (Extra fast, Normal, Slow, etc.).

.

Easing
ℹ️ Definición
Con ease, podemos darle vida a la emoción al proveer aceleraciones y ritmos personalizados al movimiento.

.
Cuando hablamos de ease tenemos que mencionar las curvas de bezier, las cuales describe 3 tipos: default-ease (personalizado), ease-in, and ease-out.
.
Así mismo, podemos organizar nuestra animación mediante el tipo (t1 ease-in) o, a través de una expresión funcional para describir un movimiento fino (Expressive easing ) para switches o checks, así como para describir un movimiento productivo (Productive easing) para modales o alertas.
.

Efectos
ℹ️ Definición
Un efecto es la propiedad de un objeto que lo distingue de uno estático.

.
Cuando un efecto es aplicado a un componente, se convierte en un elemento de interacción que posee un inicio y un final.
.
Para sistematizar estos efectos, se puede usar la convención de nombres que describe su fin, es decir, el estado inicial animate-in o el final animate-out . O por elección, nombrar mediante el efecto descriptivo que realizará Card fade-in .
.

Coreografía
ℹ️ Definición
Una coreografía es definida al acto donde múltiples objetos forman parte, simultáneamente, en un movimiento dado.

.
Por último, podemos mencionar que una animación es el resultado orquestado de una coreografía que, en acto, definirá un fin:
.

Complejidad
Basado en la cantidad de bloques que se complementan entre sí
.
Principio base
Los usuarios están concentrados en un contexto espacial
.
Narrativa
Mediante un flujo de trabajo (user journey)
.
Accesibilidad
El movimiento está mantenido en contenedores en su lugar de elementos