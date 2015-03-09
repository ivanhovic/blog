---
layout: post
title:  "Hosting gratuito con Heroku"
date:   2015-02-24 18:46:47
comments: true
---
#¿Qué es Heroku?#
[Heroku] es una plataforma que permite correr aplicaciones web en la nube. Esas aplicaciones pueden estar desarrolladas en Ruby, PHP, JS, Python, Java...
<!--![My helpful screenshot]({{ site.url }}/assets/Heroku_logo.png)-->

#La idea#
Sin embargo, además de poder ejecutar tus aplicaciones en todos esos lenguajes, también podrás con un simple truco, alojar una simple web estática (HTML, CSS y JS).

#El proceso#
Lo primero será darnos de alta en Heroku y crear una aplicación nueva desde el *dashboard*.

Después, será imprescindible descargar e instalar [Heroku toolbelt] y [Git].
Para comprobar si este paso está bien, entra en el terminal y escribe `heroku`y `git`. Si te sale algo parecido a lo de la imagen, estará bien:

Ahora tan sólo deberemos renombrar nuestro index.html y cambiar la extensión a php (index.html --> index.php). Con ello, Heroku creerá que estamos creando una aplicación con PHP.

El último paso será subir nuestra web a Heroku:

* `cd web_ejemplo` // Accedemos al directorio que contiene nuestros archivos con el comando `cd`.
* `git add .`  // Añadimos todos los ficheros a Git.
* `git commit -m "subida a Heroku"` // Hacemos un *commit* de nuestros ficheros.
* `git push heroku master` // Lo subimos a Heroku.

#Dominio#
Si todo ha ido bien, la web estará disponible en **ejemplo.herokuapp.com**.

Si por el contrario ya disponemos de nuestro propio dominio, será fácil redirigirlo a Heroku:
- Agregar nuestro dominio en el dashboard de nuestra App.
- Cambiar la configuración **DNS** en nuestro proveedor de dominios. En el registro **CNAME (WW)** poner **example.herokuapp.com.**


[Heroku]: http://heroku.com
[Heroku toolbelt]: https://toolbelt.heroku.com/
[Git]: http://git-scm.com/
