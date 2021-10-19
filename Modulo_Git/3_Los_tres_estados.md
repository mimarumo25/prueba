# Los tres estados
Git tiene tres estados principales en los que se pueden encontrar tus archivos: 
***confirmado (committed)***, ***modificado (modified)***, y ***preparado (staged)***.
> ***Confirmado*** significa que los datos están almacenados de manera segura en tu base de datos local. <br/>
> ***Modificado*** significa que has modificado el archivo pero todavía no lo has confirmado a tu base de datos.  <br/>
> ***Preparado*** significa que has marcado un archivo modificado en su versión actual para que vaya en tu próxima confirmación.  <br/>

Esto nos lleva a las tres secciones principales de un proyecto de Git: el directorio de Git ***(Git directory)***, el directorio de trabajo ***(working directory)***,
y el área de preparación ***(staging area)***.
![image](https://user-images.githubusercontent.com/30872921/134584264-922f95e4-2f96-481c-bb52-1f7145d6d866.png)

El directorio de Git es donde se almacenan los metadatos y la base de datos de objetos para tu proyecto. Es la parte más importante de Git, y es lo que se copia cuando
clonas un repositorio desde otra computadora. El directorio de trabajo es una copia de una versión del proyecto. Estos archivos se sacan de la base de datos comprimida 
en el directorio de Git, y se colocan en disco para que los puedas usar o modificar.
El área de preparación es un archivo, generalmente contenido en tu directorio de Git, que almacena información acerca de lo que va a ir en tu próxima confirmación. A veces 
se le denomina índice (“index”), pero se está convirtiendo en estándar el referirse a ella como el área de preparación.

El flujo de trabajo básico en Git es algo así:
- Modificas una serie de archivos en tu directorio de trabajo.
- Preparas los archivos, añadiéndolos a tu área de preparación.
- Confirmas los cambios, lo que toma los archivos tal y como están en el área de preparación y almacena esa copia instantánea de manera permanente en tu directorio de Git.
