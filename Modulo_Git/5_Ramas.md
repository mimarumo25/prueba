# Ramas
Una rama representa una línea independiente de desarrollo. Las ramas sirven como una abstracción de los procesos de cambio, preparación y confirmación. Puedes concebirlas como una forma de solicitar un nuevo directorio de trabajo, un nuevo entorno de ensayo o un nuevo historial de proyecto. Las nuevas confirmaciones se registran en el historial de la rama actual, lo que crea una bifurcación en el historial del proyecto.
![image](https://user-images.githubusercontent.com/30872921/134778746-275e4d58-3613-47fa-bcbe-cf12e38e2512.png)

## Opciones comunes
`git branch` Enumera todas las ramas de tu repositorio. Es similar `a git branch --list`.

`git branch <branch>`
Crea una nueva rama llamada *branch*. Este comando no extrae la nueva rama.

`git branch -d <branch>`
Elimina la rama especificada. Esta es una operación segura, ya que Git evita que elimines la rama si tiene cambios que aún no se han fusionado.

`git branch -D <branch>`
Fuerza la eliminación de la rama especificada, incluso si tiene cambios sin fusionar. Este comando lo puedes usar si quieres eliminar de forma permanente todas las confirmaciones asociadas con una línea concreta de desarrollo.

`git branch -m <branch>`
Cambia el nombre de la rama actual a *branch*.

`git branch -a `
Enumera todas las ramas remotas.

## Crear una nueva rama
Cuando vamos a trabajar en una nueva funcionalidad, es conveniente hacerlo en una nueva rama, para no modificar la rama principal y dejarla inestable. Aunque la orden para
manejar ramas es `git branch` podemos usar también `git checkout`.
```
$ git branch hola
$ git checkout hola
Switched to branch 'hola'
```

O de forma más rápida:
```
$ git checkout -b hola
Switched to a new branch 'hola'
```

## Modificaciones en la rama secundaria 
Añadimos un nuevo archivo en el directorio newRama llamado HolaMundo.hmtl:
1. Verificar el nombre de la rama donde estamos ubicados `$ git branch`
2. Si esta en la rama master o main debemos canviarnos de rama con el momando `$ git checkout hola` 
3. Agregar los cambio $ git add newRama/HolaMundo.html
4. `$ git commit -m` "Añadida la clase HolaMundo"
5. Tenemos la información en el putnero deseado.
