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
Usa la metodología BEM de manera consistente en todos tus proyectos.
