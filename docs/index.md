En el congreso UseR! del 2019 en la Ciudad de México, fuí testigo de varias presentaciones realizadas en R. De esto me 
surgio la duda de cual era mi librería favorita. Recorde haber usado **RevealJS** junto con una sensación de 
complejidad. También recorde a **Slidy** e **IoSlide**, mas no tenía claro porque razón en aquella ocasión decidí dejarlas
de lado. Por lo tanto me dí a la tarea de realizar el ejercicio con las librerías disponibles.

Espero pueda ser de útilidad para alguien mas y cualquier comentario es bienvenido en el repositorio.

## IoSlides

Presentaciones con la librería **IoSlides**.
Hasta el momento me parece la mas sencilla con una resultado bien logrado. Soporta gráficas interactivas, ggplot y una 
buena detección de sintaxis. Me gusta mucho como centra los gráficos y la transición entre diapositivas. Quiza es la librería
mas sencilla de implementar en un flujo de trabajo cotidiano.

[Presentación base](presentacion-ioslides.html)

## Beamer

Presentaciones realizadas con **Beamer**.
Esta librería genera un archivo **PDF** que tiene como ventaja la portabilidad, donde lo ejecutemos se verá igual. Sin 
embargo no permite la ejecución de gráficas interactivas. Aunque usando servicios WEB como **SlideShare** o **SpeakerDeck**,
que permiten mostrar en línea las diapositivas exportadas en PDF. Si bien tiene temas que podemos aplicar, la estética de la
presentación base no es la mas bonita del grupo. Ademas requiere de una instalación **completa** de Latex para poder 
generar el archivo PDF, lo que implica una instalación de varios megas.

[Presetación base](presentacion-beamer.pdf)

## Slidy

Presentaciones usando **Slidy**.
Las presentaciones generadas con esta librería son un poco mas ligeras, se ejecuta con la misma facilidad que las 
**IoSlides**, la configuración base permite transiciones sencillas y un scroll hacíá abajo.
Sin embargo la estructura y estética es un tanto extraña, me parece que no se distribuye bien sobre cada diapositiva y
la transición así como los colores no estan tan trabajados como en **Ioslides**. De hecho la distribución sobre la 
diapositiva se debe a los espacios y saltos de línea. Estructurando los parrafos desde **Rmarkdown**.

[Presetación base](presentacion-slidy.html)

## RevealJS

Presentaciones usando **RevealJS**.

RevealJS tiene la configuración base mas cuidada de todas las alternativas. Aunque también es la mas pesada. Requiere pocas 
configuraciones que resultan en animaciones muy bonitas y tiene una vista panoramica de las diapositivas. 
No me encanta como estructura el texto y hay que poner atención especial en que el texto quede dentro de la diapositiva 
para que no se corte, o en su defecto activar usar diapositivas verticales. La presentación es bonita y llamativa. 
La animación que presenta directamente es muy estética, la posibilidad de ver una panorámica de todas las diapositivas 
parece realmente útil.

[Presetación base](presentacion-revealjs.html)

## Xaringan

Presentación usando **Xaringan**.

Es la libreríá mas configurable, tiene muchas opciones y su integración con **javascript** y **CSS** es transparente.
La sintaxis cambia un poco, deja de usar los títulos y usa guiones `---` para delimitar las diapositivas.
Tiene muchas opciones de configuración, acepta **footnotes** y **dos columnas** de forma nativa. Al inicio de la 
diapositiva se puede definir la justificación del texto así como la imagen de fondo. Se pueden agregar notas para el 
presentador y una ejecución automática con temporizador así como un contador en pantalla.

Ademas se pueden separar elementos para que se muestren paso a paso usando dos guiones en vez de tres. Puede resaltar
líneas dentro de chunks de código usando asteriscos, llaves dobles e incluso **#<<**. Hasta se pueden declarar rangos de
página.
Por último se integra directamente con hojas de estilo (CSS), por lo que es completamente configurabley cuenta con varios
**temas**.

El tamaño esta por arriba de las **Ioslides** pero no tan grande como la presentación **revealjs**, ademas de que por 
default el output no es autocontenido. En este caso, cuando el archivo no es autocontenido, no se puede ver en el visor
de **Rstudio** y solo hasta que se crea un output autocontenido se puede visualizar directamente.

[Presetación base](presentacion-xaringan.html)
