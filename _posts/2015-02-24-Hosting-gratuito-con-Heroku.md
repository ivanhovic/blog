---
layout: post
title:  "Hosting gratuito con Heroku"
date:   2015-02-24 18:46:47
comments: true
---
#¿Qué es Heroku?#
[Heroku] permite construir y correr aplicaciones web hechas en PHP, Python, Ruby, Java...
![My helpful screenshot]({{ site.url }}/assets/Heroku_logo.png)

#La idea#
Sin embargo, además de poder ejecutar tus aplicaciones en todos esos lenguajes, también podrás con un simple truco, alojar una simple  web estática (HTML, CSS y JS).

#El proceso#
Lo primero será darnos de alta en Heroku y crear una aplicación desde el propio dashboard.
Además, deberemos bajarnos e instalar [Heroku toolbelt] y [Git].

Deberemos renombrar nuestro index.html y cambiarlo a index.php.
Para subir nuestra web a Heroku deberemos hacer un commit con git y agregar los cambios a la rama de Heroku.

* `cd web_ejemplo`
* `git add .`
* `git commit -m "make it better"`
* `git push heroku master

#Dominio#
Si ya teniamos nuestro propio dominio será fácil agregarlo. Simplemente deberamos agregarlo en el dashboard de nuestra App y cambiar la configuración CNAME en nuestro proveedor de dominios.


#Problemas#


[Heroku]: http://heroku.com
[Heroku toolbelt]: https://toolbelt.heroku.com/
[Git]: http://git-scm.com/
