https://www.youtube.com/c/TailwindLabs/videos
https://www.figma.com/file/aPbr2Rhd5SCUjNYu6NRPPB/Platzi-Travel-Mockups?node-id=0%3A1&mode=dev



Es importante que veas esto si estás viendo el curso con la versión 3 porque mucha de la documentación que vemos en esta parte no existe y además no se profundizó demasiado o a mi parecer no estuvo muy claro, es por ello que les dejo esta explicación.

Directivas de Tailwind CSS
@tailwind base
Se encarga de inicializar todos los elementos HTML sin estilos, Es decir que un botón no va a tener estilos de botón y solo va a parecerse a un texto, o que un hipervínculo no va a tener decoraciones, entre otras cosas

@tailwind component
Permite acceder a todas las clases de tailwind enfocadas a componentes, por ejemplo para un botón o similares.

@tailwind utilities
Son todos los estilos de tailwind y el núcleo del mismo, nos permite accede a clases como bg-red-500.

@apply
Se utiliza para aplicar una serie de utilidades tailwind en un selector css específico. En este caso podemos aplicar una serie de utilidades para una clase botón.

.btn {
  @apply py-2 px-4 rounded-lg bg-blue-500 text-white font-semibold;
}
@layer
Permite decir a que directiva o capa de tailwind(base,component,utilities) pertenecen las utilidades tailwind que fueron seleccionadas con la directiva apply. Por ejemplo, si queremos que por defecto nuestros headers tengan un cierto estilo cuando usamos tailwind, puede verse de esta forma.

@layer base {
  h1 {
    @apply text-2xl;
  }
  h2 {
    @apply text-xl;
  }
}
@config
Esta directiva permite especificar cual es el archivo de configuración que tailwind utilizará para compilar el archivo CSS. Esto es muy útil cuando usamos proyectos que necesitan varios archivos de configuración para diferentes archivos CSS. Por ejemplo si tenemos estilos distintos en la vista de un admin y del sitio base. Algo muy importante es no poner esta directiva antes de las declaraciones de importación porque es posible que no se apliquen estilos correctamente debido a que si estás usando postcss-import, tus declaraciones @import deben venir antes de @config para que todo funcione correctamente, ya que postcss-import sigue estrictamente las especificaciones CSS que requieren que las declaraciones @import precedan a cualquier otra regla en el archivo.

@config "./tailwind.site.config.js";
@config "./tailwind.admin.config.js";


También se puede agregar colores arbitrarios sin necesidad de configurarlos manualmente.

<button class="bg-[#1da1f2] text-white ...">Share on Twitter</button>

Un breakpoint es el salto en el que cambia la pantalla de layout. Se pueden manipular los estilos de nuestro archivo en función al tipo de dispositivo.

Debido a que Tailwind es mobile first, todo el tiempo se estará trabajando con el breakpoint small.

Breakpoints más comunes:

320px → Small → Dispositivo mobile.
768px → Medium → Tablet.
1280px → Large → Computadora.

sm - 640px
md - 768px
lg - 1024px
xl - 1280px
2xl - 1536px

Documentación oficial de Width
Documentación oficial de height

Ejemplo práctico

<div class=“w-auto h-screen bg-sky-200 flex”>
<div class=“w-1/4 h-1/4 bg-sky-700”></div>
<div class=“w-1/4 h-1/4 bg-cyan-400”></div>
<div class=“w-1/3 h-1/4 bg-cyan-700”></div>
<div class=“w-1/4 h-1/4 bg-cyan-900”></div>
</div>