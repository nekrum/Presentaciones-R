---
layout: default
---

En el congreso UseR! del 2019 en la Ciudad de México, fuí testigo de excelentes presentaciones realizadas directamente en **R**.
Esto me recordo el debate interno que tengo cada ves que decido que lirebría usar. Por lo tanto decidí, de una vez por
todas, recopilar y probar las librerías que alguna vez he usado.
Recuerdo haber usado **RevealJS** junto con una sensación de complejidad. También recorde a **Slidy** e **IoSlide**,
mas no tenía claro porque razón decidí dejarlas de lado. No he probado **Xaringan** pero aprovechare para conocerlo.
Por lo tanto me dí a la tarea de realizar el ejercicio con las librerías disponibles, con el afan de consultar mi decisión
e incluso tener disponible un archivo de ejemplo listo para usarse.

Espero pueda ser de útilidad para alguien mas y cualquier comentario es bienvenido en el repositorio.

## Presentaciones con la librería **IoSlides**.

Hasta el momento me parece la mas sencilla con una resultado bien logrado. Soporta gráficas interactivas, ggplot y una
buena detección de sintaxis. Me gusta mucho como centra los gráficos y la transición entre diapositivas. Quiza es la librería
mas sencilla de implementar en un flujo de trabajo cotidiano.

[Presentación base](presentacion-ioslides.html)

## Presentaciones realizadas con **Beamer**.

Esta librería genera un archivo **PDF** que tiene como ventaja la portabilidad, donde lo ejecutemos se verá igual. Sin
embargo no permite la ejecución de gráficas interactivas. Aunque usando servicios WEB como **SlideShare** o **SpeakerDeck**
podríamos tener una visibilidad en línea, esto no resuelve la falta de interacción con la presentación.
Esta librería tiene temas que podemos aplicar, la estética de la presentación base no es la mas bonita del grupo.
Ademas requiere de una instalación **completa** de Latex para poder generar el archivo PDF, lo que implica una
instalación de varios megas.

[Presetación base](presentacion-beamer.pdf)

## Presentaciones usando **Slidy**.

Las presentaciones generadas con esta librería son un poco mas ligeras y se ejecuta con la misma facilidad que las
**IoSlides**, la configuración base permite transiciones sencillas y se puede tener  un scroll hacia abajo en cada diapositiva.
Sin embargo la estructura y estética es un tanto extraña, me parece que no se distribuye bien sobre cada diapositiva y
la transición así como los colores no estan tan trabajados como en **Ioslides**. De hecho la distribución sobre la
diapositiva se debe a los espacios y saltos de línea que introducimos en los parrafos desde **Rmarkdown**.

[Presetación base](presentacion-slidy.html)

## Presentaciones usando **RevealJS**.

RevealJS tiene la configuración base mas cuidada de todas las alternativas, aunque también es la mas pesada.
Requiere una configuración ligera que resultan en animaciones muy bonitas.
No me encanta como estructura el texto y hay que poner atención especial en que el texto quede dentro de la diapositiva
para que no se corte, o en su defecto activar usar diapositivas verticales o sea secciones que se despliegan hacia abajo.
La presentación es bonita y llamativa, la animación que presenta directamente es muy estética, la posibilidad de ver una
panorámica de todas las diapositivas al presionar *Escape* parece realmente útil.

[Presetación base](presentacion-revealjs.html)

## Xaringan

Presentación usando **Xaringan**.

Es la libreríá mas configurable, tiene muchas opciones, su integración con **javascript** y **CSS** es transparente y presenta
varios **temas**.
La sintaxis cambia un poco, deja de usar los títulos y usa guiones `---` para delimitar las diapositivas.
Tiene muchas opciones de configuración, acepta **footnotes** y **dos columnas** de forma nativa. Al inicio de la
diapositiva se puede definir la justificación del texto así como la imagen de fondo. Se pueden agregar notas para el
presentador y una ejecución automática con temporizador así como un contador en pantalla.

Ademas se pueden separar elementos para que se muestren paso a paso usando dos guiones en vez de tres. Puede resaltar
líneas dentro de chunks de código usando asteriscos, llaves dobles e incluso **#<<**. Hasta se pueden declarar rangos de
renglones que se necesiten resaltar.

El tamaño esta por arriba de las **Ioslides** pero no tan grande como la presentación **revealjs**, ademas de que por
default el output no es autocontenido. En este caso, cuando el archivo no es autocontenido, no se puede ver en el visor
de **Rstudio** y solo hasta que se declara se puede visualizar directamente.


[Presetación base](presentacion-xaringan.html)

# Conclusiones

De manera genera puedo decir que para presentaciones en un flujo continuo y que permitan una estética bonita sin complicaciones
usaría la librería **IoSlide**, porque requiere poca configuración y se encarga de la estructura de forma casí transparente.

Para presentaciones mas cuidadas que tengan un efecto **WOW** no estoy seguro. Creo que **RevealJS** hace un gran trabajo
y no necesita tanta configuración. Su animación es llamativa y tenemos una buena presentación sin demasiada configuración.
**Xaringan** por otro lado no tiene animaciones ta trabajadas, pero tiene muchos elementos extra que me llamaron la atención.
Desde las notas para presentador, el reloj contador, el resaltado dentro de código notas al pie, que lo hacen una alternativa
llamativa. Es verdad que algunos de estos elementos se puede generar el **RevealJS** pero se vuelve complejo y difícil de
implementar.
