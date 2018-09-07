
# Flujo de trabajo en Git

Es importante que cuando varios desarrolladores trabajan en un mismo proyecto, versionado con ***Git***, esté bien definido un flujo de trabajo y de ramificaciones.
!["Git"](https://www.soe.uagrm.edu.bo/wp-content/uploads/2017/05/git-github.jpg)

Ya sabemos que ***Git*** es un sistema de control de versiones distribuido en el que cada desarrollador es un repositorio independiente, aunque en algún caso se cuente con un repositorio central, en el que el trabajo con ramas es extremadamente sencillo, pudiendo mantener a la vez distintas ramas abiertas, usándolas en diferentes momentos del desarrollo y fusionándolas con frecuencia. Dada la facilidad para trabajar con ramas en Git, hay que ser cuidadosos y no caer en el error de crear ramas descontroladamente haciendo que el repositorio resulte caótico.

Los 3 comandos básicos para agregar nuestro proyecto a Git, son:

~~~
git add .
git commit -m "Nombre de la nueva versión"
git push -u origin master
~~~
Pero, ¿qué significa "***add***" y "***commit***"? ¿Por qué pasamos por estas dos fases?

!["Ejemplo"](https://cdn-images-1.medium.com/max/686/1*diRLm1S5hkVoh5qeArND0Q@2x.png)

Ya habíamos visto anteriormente las fases de git, sino echale un vistazo a [GIT](https://github.com/PaulaSshun/tatooine/tree/master/SPRINT-2/01-GIT).

Nuestro repositorio local tiene 3 diferentes fases por la cual pasa nuestro código:

1. **Working directory:** En esta parte podemos hacer cualquier cambio y no afectar nuestro repositorio.
2. **Staging area:** Archivos modificados.
3. **Git repository:** Archivos confirmados.

El código tiene 3 status en cada diferente fase, las más comunes son:
1. **Modified**
2. **Staged**
3. **commited**

Cuando modificamos algo de nuestro código, se vuelve en status **modificado**.
Comprobamos esto con el comando **git status**, así veremos cuando un archivo ha sido modificado o creado.

!["Untrack file"](file:///Users/HDH-V/Desktop/SSdeLaTerminal.png "**Untrackedfiles** es para archivos recién creados y **modified** para los modificados")

Después de que hicimos los cambios necesarios pasamos a la siguiente etapa ***Staging Area***

~~~
git add .
~~~
 Es lo mismo que poner:

~~~
git add NombreDelArchivo.text
~~~
Ahora todos los archivos modificados dentro de **Working directory** los pasamos a **Staging Area**.

Este estado del código pasa de **modificado** a **preparado**.

A continuación pasamos a la parte de **"Staging Area"**. En esta parte podemos dar nombre a la nueva versión.

Aún no se publica en github. Para pasar a la fase siguiente de nuestro código (*de Staging Area al Git repository*), escribimos lo siguiente.

~~~
git commit -m "Algún comentario"
~~~
*Nótese que "-m" significa que le vamos a agregar un comentario.*

Ahora el código pasa de preparado a confirmado.

Una vez que el código está confirmado ya está listo para sincronizarse con el servidor de Git (en este caso es github). Para hacerlo, escribimos:

~~~
git push origin *nombre del branch*
~~~
*Pushea baby pushea!*

Cuando trabajamos un repositorio con varias personas se tiene que descargar los cambios que hizo esa persona, pero ojo, si dos personas la mismo tiempo tratan de meter push en el repositorio mandará un mensaje de que tenemos que primero descargar la versión  de la persona que hizo el primer push para después juntarlo y subirlo.

Para eso ejecutamos:

 ~~~
 git pull origin master
 ~~~
*pulea baby pulea!*

Este proceso pasa por un **checkout the proyect**.

Aquí un ejemplo de lo que acabo de explicar.

!["Flujo de git"](https://cdn-images-1.medium.com/max/800/1*D1lbqiz2Y6quKrt00p9DqQ.png)

Bien, ahora estás list@  para pulear y pushear, así que a perder el miedo a romper las cosas!
