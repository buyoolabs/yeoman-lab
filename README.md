yeoman-lab
==========

     _-----_
    |       |
    |--(o)--|   .--------------------------.
   `---------´  |    Welcome to Yeoman,    |
    ( _´U`_ )   |   ladies and gentlemen!  |
    /___A___\   '__________________________'
     |  ~  |
   __'.___.'__
 ´   `  |° ´ Y `

# Yeoman

- *Yeoman* es una herramienta para ayudar con el *workflow* de desarrollo web, sobre todo sirve de lanzadera para crear un nuevo proyecto
- Yeoman se compone de tres herramientas:
	- [yo](http://yeoman.io/): para hacer scaffolding, para generar un punto de partida
	- [bower](http://bower.io/)*: un gestor de paquetes, por ej: agregar frameworks o herramientas de manera sencilla
	- [grunt](http://gruntjs.com/): una herramienta de generación de tareas automáticas, por ej: compilar ficheros Sass u optimizar imágenes
- Requiere Node.js, para instalarlo: `npm install -g yo`
- La interfaz es línea de comandos en el terminal, para cualquiera de las 3 herramientas
- Tiene cientos de generadores predefinidos: WebApp, AngularJS, FirefoxOS, Wordpress, Cordova...
	- Por ejemplo, para generar una webapp normal con html5, jquery y bootstrap: 
		- Para instalar el paquete: `npm install -g generator-webapp`
		- Para lanzar el generador (sobre una carpeta): `yo webapp`
- Grunt tiene tareas populares predefinidas en: [https://github.com/gruntjs/grunt-contrib](http://gruntjs.com/). Algunas de estas tareas son:
	- Limpieza de ficheros y carpetas
	- Compilar CoffeScript
	- Compilar Compass
	- Lanzar jshint/jslint
	- Concatenar ficheros
	- Minificar ficheros
	- Optimizar imágenes para web
	- Ejecutar tests unitarios javascript
- Un ejemplo completo para crear una webapp (proyecto adjunto yo-demo):
	- `$ mkdir yo-demo`
	- `$ cd yo-demo`
	- `$ yo webapp`
	- `$ bower install`
	- `$ grunt build`
	- `$ grunt serve`
	- Esto dará como resultado la creación de una carpeta "dist" con el resultado de las operaciones, y lo pondrá en marcha en un server local


# Conclusiones

- Para nuestro flujo normal de trabajo, Yo y Bower no nos serán especialmente últiles:
	- yo se orienta a la creación de nuevos proyectos de una manera ágil
	- bower es un gestor de paquetes, nosotros ya usamos NuGet integrado con Visual Studio
- Grunt si nos puede llegar a ser útil en diversas tareas como:
	- Optimización automática de imágenes para web antes de un release
	- Minimificación de html/aspx antes de una release
	- Tareas automatizadas personalizadas
