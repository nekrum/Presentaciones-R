# Comparativa de Presentaciones en R

Código base para crear presentaciones con R, estan escritos en Rmarkdown, para instalar las librerías necesarias
podemos ejecutar en **Rstudio** o en **R-base**

```
source('requerimientos.R')
```

En la carpeta **docs** se crea un sitio para mostrar las presentaciones y pequeños resumenes.

Para mostrar localmente el sitio, se necesita instalar `ruby`, `bundler` y `rake`.

- `ruby`: Es el lenguaje en el cual corre el servidor **jekyll**
- `bundler`: Permite gestionar las dependencias de las diferentes gemas que necesitamos.
- `rake`: Permite gestionar y automatizar tareas

Para instalar bundler:

```
gem install bundler
```

Para instalar las dependencias, necesitamos un archivo **Gemfile** que contenga las gemas que vamos a instalar y en el
directorio se ejecuta:

```
bundle install
```

Ademas necesitamos un **Rakefile** donde se describa los parametros que ejecuta la tarea.
Para correr el servidor localmente en [http://localhost:4000](http://localhost:4000) ejecutamos:

```
bundle exec rake servidor
```
## Resultado

Para acceder a la pagina:

https://nekrum.github.io/Presentaciones-R/
