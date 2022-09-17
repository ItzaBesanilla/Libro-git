# Comandos para la realización de ejercicios.

### **A continuación se van a mostrar los comandos utilizados para poder realizar todos los ejercicios planteados.**


## - CREACIÓN Y ACTUALIZACIÓN DE GIT.

**Ejercicio 1.**

Configurar Git definiendo el nombre del usuario, el correo electrónico y activar el coloreado de la salida. Mostrar la configuración final.

    git config --global user.name = ""
    git config --global user.email = ""
    git config --global color.ui auto

Ejemplo:

![](https://github.com/ItzaBesanilla/Libro-git/blob/1cc15b46815d138be34ac03f40d8dabbead55f9d/Ejercicios/1-%20Creaci%C3%B3n%20y%20actualizacion/Configurar%20nombre%20y%20correo.png)

**Ejercicio 2.**

Crear un repositorio nuevo con el nombre libro y mostrar sus contenido.

    git init 
	ls -lha

![](https://github.com/ItzaBesanilla/Libro-git/blob/1cc15b46815d138be34ac03f40d8dabbead55f9d/Ejercicios/1-%20Creaci%C3%B3n%20y%20actualizacion/iniciar%20repositorio.png)

![](https://github.com/ItzaBesanilla/Libro-git/blob/master/Ejercicios/1-%20Creaci%C3%B3n%20y%20actualizacion/Mostrar%20contenido.png)

**Ejercicio 3.**

1. Comprobar el estado del repositorio.
    git status
 
 ![](https://github.com/ItzaBesanilla/Libro-git/blob/1cc15b46815d138be34ac03f40d8dabbead55f9d/Ejercicios/1-%20Creaci%C3%B3n%20y%20actualizacion/Comprobar%20estado%20del%20repositorio.png)
 
2. Crear un fichero indice.txt con el siguiente contenido:

Capítulo 1: Introducción a Git

Capítulo 2: Flujo de trabajo básico

Capítulo 3: Repositorios remotos

     cat  indice.txt
     nano indice.txt
    
![](https://github.com/ItzaBesanilla/Libro-git/blob/1cc15b46815d138be34ac03f40d8dabbead55f9d/Ejercicios/1-%20Creaci%C3%B3n%20y%20actualizacion/Crear%20un%20fichero.png)

1. Comprobar de nuevo el estado del repositorio.
2. Añadir el fichero a la zona de intercambio temporal.
3. Volver a comprobar una vez más el estado del repositorio.


    git status
    
    git add .
    
	  git status

![](https://github.com/ItzaBesanilla/Libro-git/blob/1cc15b46815d138be34ac03f40d8dabbead55f9d/Ejercicios/1-%20Creaci%C3%B3n%20y%20actualizacion/Guardar%20y%20mostrar%20cambios.png)

**Ejercicio 4.**

Realizar un commit de los últimos cambios con el mensaje “Añadido índice del libro.” y ver el estado del repositorio.

     git commit -m "Añadido indice del libro."

![](https://github.com/ItzaBesanilla/Libro-git/blob/7b6f16eb4f27249cc3e4c45d24bdcf12352e4f34/Ejercicios/1-%20Creaci%C3%B3n%20y%20actualizacion/Hacer%20commit.png)

1. Mostrar los cambios de la última versión del repositorio con respecto a la anterior.
2. Cambiar el mensaje del último commit por “Añadido capítulo 3 sobre gestión de ramas al índice.”
3. Volver a mostrar los últimos cambios del repositorio.



     git commit -amend "Añadido capítulo 3 sobre gestión de ramas al índice.
    
     git show
     
     

![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/1-%20Creaci%C3%B3n%20y%20actualizacion/Modificar%20commit%20realizado.png)

![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/1-%20Creaci%C3%B3n%20y%20actualizacion/Mostrar%20ultimos%20cambios.png)


## - HISTORIAL DE CAMBIOS.

**Ejercicio 1.**

1. Mostrar el historial de cambios del repositorio.



     git log

![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/1-Mostrar%20historial%20de%20cambios.png)


2. Crear la carpeta capitulos y crear dentro de ella el fichero capitulo1.txt con el siguiente texto.
> Git es un sistema de control de versiones ideado por Linus Torvalds.


     mkdir capitulos
	 cat > capitulos/capitulo1.txt

![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/2-%20crear%20carpeta%20capitulos%20con%20fichero.png)

3. Añadir los cambios a la zona de intercambio temporal.


    git add .
    
![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/3-%20A%C3%B1adir%20cambios%20a%20zona%20temporal.png)

4. Hacer un commit de los cambios con el mensaje "Añadido capitulo 1."


    git commit -m "Añadido capitulo 1."

![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/4-%20Hacer%20commit.png)

5. Volver a mostrar el historial de cambios del repositorio.


    git log

![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/5-%20Mostrar%20historial%20de%20cambios.png)

**Ejercicio 2.**

1. Crear el fichero capitulo2.txt en la carpeta capitulos con el siguiente texto.
>El flujo de trabajo básico con Git consiste en: 1- Hacer cambios en el repositorio. 2- Añadir los cambios a la zona de intercambio temporal. 3- Hacer un commit de los cambios.


    cat > capitulos/capitulo2.txt


![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/6-%20Crear%20fichero2,%20a%C3%B1adir%20cambios%20y%20hacer%20commit.png)


2. Añadir los cambios a la zona de intercambio temporal.


    git add .

![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/7-%20A%C3%B1adir%20cambios%20a%20zona%20temporal.png)

3. Hacer un commit de los cambios con el mensaje "Añadido capitulo 2."


    git commit -m "Añadido capitulo 2."

![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/8-%20Hacer%20commit%20capitulo%202.png)


4. Mostrar las diferencias entre la última version y dos versiones anteriores.


    git diff HEAD~2..HEAD


![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/9-%20Mostrar%20diferencia%20entre%20ultima%20y%20las%20versiones%20anteriores.png)


**Ejercicio 3.**

1.  Crear el fichero capitulo3.txt en la carpeta capitulos con el siguiente texto.

> Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas.


    cat > capitulos/capitulo3.txt

![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/10-%20Crear%20capitulo3.png)


2. Añadir los cambios a la zona de intercambio temporal.


     git add .


3. Hacer un commit de los cambios con el mensaje "Añadido capitulo 3."


     git commit -m "Añadido capitulo 3,"

![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/12-%20Hacer%20commit.png)

4. Mostrar las diferencias entre la primera y última versión del repositorio.

>Primero se pone git log para ver el historial de commits que se han hecho y así poder copiar los primeros 5 caracteres del primer hash realizado.
Después esos 5 caracteres se comparan con el Head que es el último commit realizado.


    git log
	git diff a6a67e..HEAD


![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/13-1%20mostrar%20diferencia%20entre%201%C2%B0%20y%20ultima%20version.png)

![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/13-2%20Mostrar%20diferencia%20entre%201%C2%B0%20y%20ultima%20version.png)
    

**Ejercicio 4.**

1. Añadir al final del fichero indice.txt la siguiente línea:

> Capitulo 5: Conceptos avanzados.


     nano indice.txt

2. Añadir los cambios a la zona de intercambio temporal.


     git add .

3. Hacer un commit de los cambios con el mensaje "Añadido capitulo 5 al índice."


     git commit -m "Añadido capitulo5 al indice."

![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/15-%20Se%20a%C3%B1aden%20cambios%20y%20se%20hace%20commit.png)

4. Mostrar quien ha hecho cambios sobre el fichero indice.txt


     git annotate indice.txt

![](https://github.com/ItzaBesanilla/Libro-git/blob/a03c1e25f6e77ab13c96bc01d1524c7a159280f3/Ejercicios/2-%20Historial%20de%20cambios/16-%20Se%20muestra%20quien%20hizo%20cambios.png)

## - DESHACER CAMBIOS.

**Ejercicio 1.**

1. Eliminar la última línea del fichero indice.txt y guardarlo.


     vi indice.txt
    

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/1-Eliminar%20ultima%20linea%20del%20fichero.png)


2. Comprobar el estado del repositorio.


   git status

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/2-Comprobar%20estado%20del%20repositorio.png)


3. Deshacer los cambios realizados en el fichero indice.txt para volver a la versión anterior del fichero.


    git checkout --indice.txt

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/3-Deshacer%20cambios%20y%20volver%20a%20version%20anterior.png)

4. Volver a comprobar el estado del repositorio.


    git status

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/4-Comprobar%20estado%20del%20repositorio.png)

**Ejercicio 2.**

1. Eliminar la última línea del fichero indice.txt y guardarlo.


    nano indice.txt

2. Añadir los cambios a la zona de intercambio temporal (staging area).


    git add .

3. Comprobar de nuevo el estado(status) del repositorio.


    git status

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/7-Comprobar%20cambios.png)

4. Quitar los cambios de la zona de intercambio temporal, pero mantenerlos en el directorio de trabajo.


    git reset indice.txt

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/8-Quitar%20cambios%20y%20mantenerlos%20en%20el%20directorio%20de%20trabajo.png)

5. Comprobar de nuevo el estado del repositorio.


    git status

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/9-Comprobar%20estado.png)

6. Deshacer los cambios realizados en el fichero indice.txt para volver a la versión anterior del fichero.


    git checkout --indice.txt

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/10-%20Deshacer%20cambios%20en%20fichero%20y%20volver%20a%20la%20version%20anterior.png)

7. Volver a comprobar el estado del repositorio.

   
	git status

**Ejercicio 3.**

1. Eliminar la última línea del fichero indice.txt y guardarlo.


    nano indice.txt

2. Eliminar el fichero capitulos/capitulo3.txt.


    rm capitulos/capitulo3.txt

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/12-Eliminar%20fichero%20capitulos-capitulo3.png)


3. Añadir un fichero nuevo captitulos/capitulo4.txt vacío.


    touch capitulos/capitulo4.txt

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/13-A%C3%B1adir%20fichero%20nuevo.png)

4. Añadir los cambios a la zona de intercambio temporal.


    git add .

5. Comprobar de nuevo el estado del repositorio.


    git status

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/15-Verificar%20estado.png)

6. Quitar los cambios de la zona de intercambio temporal, pero mantenerlos en el directorio de trabajo.


    git reset

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/16-Quitar%20cambios%20de%20la%20zona%20pero%20mantenerlos%20en%20el%20directorio.png)

7. Comprobar de nuevo el estado del repositorio.


    git status

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/17-Comprobar%20estado.png)

8. Deshacer los cambios realizados para volver a la versión del repositorio.

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/18-Deshacer%20cambios%20para%20volver%20a%20la%20version%20anterior.png)

9. Volver a comprobar el estado del repositorio.

    
	git status

**Ejercicio 4.**

1. Eliminar la última línea del fichero indice.txt y guardarlo.

  
      nano indice.txt

2. Eliminar el fichero capitulos/capitulo3.txt.


    rm capitulos/capitulo3.txt

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/20-Eliminar%20fichero.png)

3. Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Borrado accidental.”


    git add . 
	git commit -m "Borrado accidental"

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/21-A%C3%B1adir%20cambios%20y%20hacer%20commit.png)

4. Comprobar el historial del repositorio.


    git log 

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/22-Comprobar%20historial%20del%20repositorio.png)


5. Deshacer el último commit pero mantener los cambios anteriores en el directorio de trabajo y la zona de intercambio temporal.


    git reset --soft HEAD~1

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/23-Deshacer%20ultimo%20commit%20y%20mantener%20los%20anteriores.png)

6. Comprobar el historial y el estado del repositorio.

    git status

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/24-Comprobar%20historial.png)

7. Volver a hacer el commit con el mismo mensaje de antes.


![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/25-Volver%20a%20hacer%20commit.png)


8. Deshacer el último commit y los cambios anteriores del directorio de trabajo volviendo a la versión anterior del repositorio.


    git reset --hard HEAD~1

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/26-Deshacer%20ultimo%20commit%20y%20cambios%20anteriores.png)


9. Comprobar de nuevo el historial y el estado del repositorio.

![](https://github.com/ItzaBesanilla/Libro-git/blob/9ce13915fcb78b12523ae39279efb574fa5c65d6/Ejercicios/3-%20Deshacer%20cambios/27-Comprobar%20de%20nuevo%20estado.png)
