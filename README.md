# git-tutorial
Git Tutorial

Hola a todos. Bienvenidos a este tutorial de Git. Vamos a crear una lista de nombres de los estudiantes de la clase. Iremos llenando la carpeta de `Nombres` con un archivo .py que tenga tu nombre, por ejemplo `mi_nombre.py`.

En el archivo llénalo con la siguiente información. Puedes utilizar como plantilla el archivo `patricio_fernandez.py`
```python

if __name__ == '__main__':
  nombre = 'Patricio F'
  print(f'Mi nombre es {nombre}')
````

No elimines, modifiques o cambies los archivos de tus compañeros. Vamos a trabajar de forma colaborativa!

Pasos a seguir: 

- Clona el repositorio (utiliza `git clone`o la app de escritorio). Verás que se crea el repositorio en local con todos los archivos necesarios.
- Vamos a crear nuestra propia rama. **ESTO ES FUNDAMNETAL**. `git checkout -b nombre_de_mi_rama_nueva`
- Entra al directorio `Nombres` (en tu local) y crea un nuevo archivo `tu_nombre.py` y complementa la información como en la plantilla. 
- Guarda el archivo y luego añade tus archivos al "tracking" de git. -> `git add .`
- Esto añade tu archivo al sistema de monitoreo de git para este repo. Si haces cambios en el archivo, podrás subirlos al repositorio remoto (origen). Luego vamos a hacer un commit de nuestros cambios. Commit significa compromiso, es decir nos comprometemos con los cambios realizados. `git commit -m "el argumento -m nos permite añadir un comentario a nuestro commit, añade el tuyo personalizado"``
- Una vez realizado el commit, vamos a subir nuestros cambios al repo remoto. Esto se hace a través de un Push. Vamos a crear la rama que tenemos en local, en remoto. Es decir, nuestros cambios estarán aparte de la rama principal y del resto de ramas de tus compañeros. Para ello ejecutamos `git push origin HEAD`. Esto empuja tus cambios a el repositorio de origen, en una nueva rama. 

Más adelante: 


- Nuestros cambios viven en una rama separada. Para fusionar nuestros cambios con la rama de origen ('main'), vamos a realizar un merge. Esto se hace a través de un pull request. Lo vamos a ver en la clase. 
- Luego, si queremos actualizar nuestro local con los últimos cambios que han subido tus compañeros (remoto), tenemos que ejecutar lo siguiente: 
````bash

git fetch 
git checkout origin/main
git pull
````

Listo! Los cambios se han actualizado en tu local.

