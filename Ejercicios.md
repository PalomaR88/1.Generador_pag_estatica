
    1. Selecciona una combinación entre generador de páginas estáticas y servicio donde desplegar la página web. Escribe tu propuesta en redmine, cada propuesta debe ser original.

Surge - Hugo

    2. Comenta la instalación del generador de página estática. Recuerda que el generador tienes que instalarlo en tu entorno de desarrollo. Indica el lenguaje en el que está desarrollado y el sistema de plantillas que utiliza. (1 punto)

HUGO: Lenguaje: JavaScript. Sistema de plantillas: React.

Instalación de Hugo:
~~~
sudo apt-get install hugo
~~~

~~~
$ hugo new site quickstart
Congratulations! Your new Hugo site is created in /home/paloma/DISCO2/CICLO II/IMPLANTACIÓN DE APLICACIONES WEB/1.Generador_pag_estatica/quickstart.

Just a few more steps and you're ready to go:

1. Download a theme into the same-named folder.
   Choose a theme from https://themes.gohugo.io/, or
   create your own with the "hugo new theme <THEMENAME>" command.
2. Perhaps you want to add some content. You can add single files
   with "hugo new <SECTIONNAME>/<FILENAME>.<FORMAT>".
3. Start the built-in live server via "hugo server".

Visit https://gohugo.io/ for quickstart guide and full documentation.
~~~

~~~
$ cd quickstart
$ git init
Inicializado repositorio Git vacío en /home/paloma/DISCO2/CICLO II/IMPLANTACIÓN DE APLICACIONES WEB/1.Generador_pag_estatica/quickstart/.git/
paloma@coatlicue:~/DISCO2/CICLO II/IMPLANTACIÓN DE APLICACIONES WEB/1.Gene
rador_pag_estatica/quickstart$ git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
Clonando en '/home/paloma/DISCO2/CICLO II/IMPLANTACIÓN DE APLICACIONES WEB/1.Generador_pag_estatica/quickstart/themes/ananke'...
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 1416 (delta 0), reused 1 (delta 0), pack-reused 1411
Recibiendo objetos: 100% (1416/1416), 4.15 MiB | 3.55 MiB/s, listo.
Resolviendo deltas: 100% (764/764), listo.
$ echo 'theme = "ananke"' >> config.toml
~~~




    3. Configura el generador para cambiar el nombre de tu página, el tema o estilo de la página,… Indica cualquier otro cambio de configuración que hayas realizado. (1 punto)
    4. Genera un sitio web estático con al menos 3 páginas. Deben estar escritas en Markdown y deben tener los siguientes elementos HTML: títulos, listas, párrafos, enlaces e imágenes. El código que estas desarrollando, configuración del generado, páginas en markdown,… debe estar en un repositorio Git (no es necesario que el código generado se guarde en el repositorio, evitalo usando el fichero .gitignore). (3 puntos)
    5. Explica el proceso de despliegue utilizado por el servicio de hosting que vas a utilizar. (2 puntos)
    6. Piensa algún método (script, scp, rsync, git,…) que te permita automatizar la generación de la página (integración continua) y el despliegue automático de la página en el entorno de producción, después de realizar un cambio de la página en el entorno de desarrollo. Muestra al profesor un ejemplo de como al modificar la página se realiza la puesta en producción de forma automática. (3 puntos)


