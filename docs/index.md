En el congreso UseR! del 2019 en la Ciudad de México, fuí testigo de varias presentaciones realizadas en R. De esto me 
surgio la duda de cual era mi librería favorita. Recorde haber usado **RevealJS** junto con una sensación de 
complejidad. También recorde a **Slidy** y **IoSlide**, mas no tenía claro porque razón en aquella ocasión decidí dejarlas
de lado. Por lo tanto me dí a la tarea de realizar el ejercicio con las librerías disponibles.

Espero pueda ser de útilidad para alguien mas y cualquier comentario es bienvenido en el repositorio.

## IoSlides

Presentaciones en con la librería **IoSlides**.
Hasta el momento me parece la mas sencilla con una resultado bien logrado. Soporta gráficas interactivas, ggplot y una 
buena detección de sintaxis. Me gusta mucho como centra los gráficos y la transición entre diapositivas.

[Presentación base](presentacion-ioslides.html)

## Beamer

Presentaciones realizadas con **Beamer**.
Esta librería genera un archivo **PDF** que tiene como ventaja la portabilidad. Donde lo ejecutemos se verá igual. Sin 
embargo no permite la ejecución de gráficas interactivas. Si bien tiene temas que podemos aplicar, la estética de la
presentación base no es la mas bonita del grupo. Ademas requiere de una instalación completa de latex.

[Presetación base](presentacion-beamer.pdf)

## Slidy

Presentaciones usando **Slidy**.
Las presentaciones generadas con esta librería son un poco mas ligeras, se ejecuta con la misma facilidad que las 
**IoSlides**, la configuración base permite transiciones sencillas y un scroll hacíá abajo.
No me agrado mucho como el texto se tiene que ajustar a la diapositiva desde **markdown**.

[Presetación base](presentacion-slidy.html)

## RevealJS

Presentaciones usando **RevealJS**.
RevealJS tiene la configuración base mas cuidada de todas las alternativas. Aunque también es la mas pesada. Pocas 
configuraciones resultan en animaciones muy bonitas y tiene una vista panoramica de las diapositivas. 
No me encanta como estructura el texto y hay que poner atención especial en que el texto quede dentro de la diapositiva 
para que no se corte, o en su defecto activar usar diapositivas verticales.

[Presetación base](presentacion-revealjs.html)

## Xaringan

Presentación usando **Xaringan**.
Es la libreríá mas configurable, tiene muchas opciones y su integración con *javascript* es transparente. Permite agregar
un timer en cada diapositiva, notas para el presentador, auto avance, notas al pie, resaltado en el código, texto a dos
columnas, diapositivas invertidas en color (excelente para marcar temas) e incluso la posibilidad de definir ciertos 
parámetros para modificar la estructura de cada diapositiva. Su problema, cambia la sintaxis de las anteriores y su 
configuración es ligeramente compleja.

[Presetación base](presentacion-xaringan.html)
