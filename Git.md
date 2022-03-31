# Git
## Introducción
 Es un *software* que permite a un equipo de desarrolladores trabajar sobre el mismo código y que se pueden compartir, cambiar o añadir datos al directorio.



Se divide en 2 principales partes o estados.

1. Local, donde guardamos archivos en nuestra computadora física
    - *Working Directory*: Aquí tenemos al directorio que guarda los archivos en nuestro almacenamiento.
    - *Staging Area*: Aquí se añaden los cambios hechos.
    - *HEAD*: Aquí se crea el *commit* que nos indica un cambio muy relevante y que ya está listo para ser subido al origen.
1. Remoto, plataforma *web* donde guardaremos los archivos
    - *Remote Origin*:  El directorio remoto donde subiremos los archivos a una plataforma web como GitHub, GitLab, BitBucket, GitKraken.
## Comandos entendidos y su funcionamiento

**Cuando queremos configurar la terminal en un inicio**
```
$ > git --version   --> Te indica la versión de git que tienes descargada
$ > git config --global user.name "Nombre de usuario"   --> Establece un nombre de usuario para quien está usando la terminal
$ > git config --global user.email usuario@gmail.com  -->establece un correo para vincular al usuario
```

**Para iniciar nuestro repositorio local**
````
$ > mkdir nombre-carpeta  --> crea un nuevo directorio el cual contendrá los archivos que queramos guardar en el ewpositorio
$ > cd nombre-carpeta     --> Te direcciona al directorio creado anteriormente
$ > touch README.md --> Crea un archivo readme el cual usarás para describir o dar información importante acerca de tu repositorio
$ > touch .gitignore --> creas el gitignore dond haremos referencia a los documentos que no queremos que se suban al repositorio remoto
$ > git init --> inicializa el repositorio
$ > git status --> te da el resumen de los cambios que tengas que hacer
````


## Crear un repositorio remoto

Para crear un repositorio remoto debemos acceder a alguna de las plataformas mencionadas anteriormente y crear un nuevo repositorio, como se muestra en el siguiente *link*:
[Tutorial sobre como crear un repositorio remoto](https://docs.github.com/es/get-started/quickstart/create-a-repo)


## Flujo en Git
![Flujo de trabajo](https://res.cloudinary.com/practicaldev/image/fetch/s--sY7WHlen--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/irirl81un0bpusbw1h54.png) 

***Working Directory***

Al crear, cambiar o añadir archivos en nuestro directorio local podemos añadir los cambios al *staging area* y prepararlos con los siguientes comandos: 

````
$ > git add nombre-archivo --> añade un archivo en específico
$ > git add --all    --> añade todos los archivos que hayan detectado algún cambio preferiblemente se usa la primer vez que añadimos un cambio
$ > git add -A       --> añade todos los archivos
$ > git add .      --> añade todos los archivos
````

***Staging Area***
Aquí nuestros archivos han aceptado los cambios y están casi listos para subirse entonces ejecutamos el siguiente comando para llegar al *head*:

````
$ > git commit -m "mensaje que describe el cambio"     --> se usa para añadir algún cambio importante que se verá reflejado en nuestro repositorio remoto
````

***Head***

Aquí nuestros archivos ya están listos para subirse al repositorio remoto, en este estado podemos seguir agregando "*commits*". 

***Remote Origin***

Ya estamos listos para subir nuestro repositorio local con uno remoto en *GitHub*.

Cuando hayamos creado el repositorio remoto en *GitHub* lo "vinculamos" a nuestro repositorio local utilizando los siguientes comandos.

````
$ > git remote add origin (Aquí copiamos y pegamos el *link* de nuestro repositorio remoto)  --> ahora ambos repositorios comparten información

````

Una vez vinculados al repositorio remoto podemos enviar los cambios que se encuentran en *Head*. Por defecto Git denomina origin a nuestro repositorio remoto y crea una rama llamada master mediante:

````

$ > git push -u origin master --> para la primera vez que subamos archivos al *origin*


$ > git push --> para añadir cambios a partir de la segunda vez
````


**Del repositorio remoto al local**

Cuando queramos descargar los cambios realizados a un repositorio remoto y usarlos en el local usaremos el siguiente comando:

````
$ > git pull -u origin master  --> la primera vez

$ > git pull  --> a partir de la segunda vez 
````


