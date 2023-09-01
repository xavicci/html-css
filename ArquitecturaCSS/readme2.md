Necesitamos que el css sea:
    - Limpio
    - Escalable
    - Mantenible

PRINCIPIOS:
    - SOLID:
        * SINGLE RESPONSABILITY PRINCIPLE: Tener una única responsabilidad
        * Open Close principle: Abiertas a extender sus funcionalidades, Cerradas a modificar
        * Liskov Substitution: Las clases derivadas deben Sustituir a las clases base sin alterar el comportamiento esperado
        * Interface Segregation: No se debe obligar a ningun código a depender de métodos que no utiliza.
        * Dependency Inversion: Módulos de alto nivel no dependan de modulos de bajo nivel.
    - DRY:
        * Dont Repeat Yourself: No repetir codigo una y otra vez en las clases
    - INMUTABILITY:
        * Objeto cuyo estado no puede ser modificado una vez creado.

Arquitectura:
    -   Como se divide el código en archivos y carpetas
    -   Como trabajamos con nuestros selectones

**************************
BEM

Las siglas BEM significan “Block, Element, Modifier” y es un enfoque para estructurar y nombrar clases CSS de manera más organizada y escalable.

Block: Componentes independientes y reutilizables que representan una entidad significativa.

Element: Partes que forman parte del bloque y no tienen uso fuera de él.

Se nombran con doble guion bajo.
Ejemplo: [Block]__[Element]

Modifier: Variaciones o estados de bloques o elementos que cambian su aspecto o comportamiento.

Se nombran con dos guiones.
Ejemplo: [Block]--[Modifer]

Estructuras que podemos encontrar:
[ Block ]
[ Block ]__[ Element ]
[ Block ]--[ Modifier ]
[ Block ]__[ Element ]--[ Modifier ]
[ Block ]--[ Modifier ]

Usa nombres de bloques descriptivos que sean fáciles de entender.
Usa nombres de elementos descriptivos que sean específicos del bloque.
Usa nombres de modificadores que sean claros y concisos.
Evita usar modificadores globales, como disabled o active.

En REACT NO SE APLICARIA LO MISMO

*********************************************************************
# ATOMIC DESIGN

Atomos ⚛️

Elementos de interfaz que no se pueden dividir más y sirve como bloques de construción

Ejemplo: Label Input Button
.

Moleculas 🦠

Son Colecciones de átomos que forman componentes de interfaz de usuario relarivamente simples

Label > Input-Button
.

Organismos 🌵

Son componentes relativamente complejos que forman secciones discretas de Interfaz

Header > Img-Nav > ul > Li-Label
.

Plantillas (Templates)📟

Colocan componentes dentro de un diseño y demuestran la estructura de contenido subyacente al diseño

Body > Header - Main - Footer
.

Páginas 📄

Aplican contenido real a las plantillas
***********************************************************************

OOCSS
OOCSS es una metodología de desarrollo de CSS que se basa en principios de programación orientada a objetos. Su objetivo es crear estilos reutilizables, modulares y mantenibles para construir interfaces de usuario eficientes y escalables. OOCSS busca separar la estructura y el diseño visual, lo que significa que los estilos que definen la apariencia visual de un elemento deben ser independientes de la estructura del HTML.

Principios de OOCSS:
Separación de estructura y diseño: Los estilos se dividen en dos categorías principales: estructura y diseño. La estructura define la disposición y el posicionamiento de los elementos, mientras que el diseño se refiere a la apariencia visual, como colores y fuentes.
Separación de contenedor y contenido: Los estilos aplicados a un contenedor no deben depender de los estilos aplicados a su contenido, y viceversa. Esto facilita la reutilización de contenedores con diferentes tipos de contenido.


****************************************************************************************
****************************************************************************************
Arquitectura SMACSS
S:SCALABLEM:MODULARA:ARQUITECTUREC:CASCADINGS:STYLES:SHEET

Categorias

Base
Estilos predeterminados
Selecectores de elementos o pseudo-clases
No Clases
No ID’s
Tamaños, Colores

Layout (Diseño o estructura de página)
Estilos para las secciones principales
Header, Footer (Se usan con id o clase)

Module (Módulos)
Fragmentos únicos que puede contener:
Prefijo
Elemento
Secundario

State (Estado)
Representa situaciones dinámicas
.is-selected

Theme (Tema)
Colores Primarios (dark mode)
Formas, bordes, sombras y demas.
Se repiten en todo el sitio

*************************************************************************************
***********************************************************************************
Arquitectura ITCSS 🛖
I:InvertedT:TrianguleCSS

ITCSS es una colección de pribcioios y metricas.

La idea es visualizar el css como un triángulo invertido en capas

Principios Basicos
    Sin ID, en css
    Patrón component UI
    Arquitectura basada en clases

Metricas
    De estilos genericos a estilos específicos
    De baja especificidad a alta especficidad
    De largo alcance a localizado

Triangulo:
    -Magnitud: Alcance e impacto en cantidad de elementos
    -Especificidad: Fuerza del selector y sus propiedades
    -Claridad: Menor abstracción en la semántica e impacto del selector


Beneficios
   - Estilos globales se comparten de manera más eficaz y eficiente
   - Disminución de batallas por especificidad
   - Menos redudancia

Capas

Settings
    * Variables globales
Tools (Solo en caso de que se usen preprocesadores)
    * Funciones globales y mixins
Generic
    * CSS comun
Elements
    * Estilos de Selectores de elementos
Objects
    * Selectores basados en clases para objetos o contenedores
Components
    * Estilos para cada componente
Trumps (triunfos)
    * Estilos de utilidad y ayuda
    * En este caso podemos usar !important

*************************************************************
La arquitectura depende de:
    * Equipo
    * Proyecto
    * Tiempo
    * Si hay o no diseño