
# Flujo de trabajo en Git

Es importante que cuando varios desarrolladores trabajan en un mismo proyecto, versionado con ***Git***, esté bien definido un flujo de trabajo y de ramificaciones.

Ya sabemos que ***Git*** es un sistema de control de versiones distribuido en el que cada desarrollador es un repositorio independiente, aunque en algún caso se cuente con un repositorio central, en el que el trabajo con ramas es extremadamente sencillo, pudiendo mantener a la vez distintas ramas abiertas, usándolas en diferentes momentos del desarrollo y fusionándolas con frecuencia. Dada la facilidad para trabajar con ramas en Git, hay que ser cuidadoso y no caer en el error de crear ramas descontroladamente haciendo que el repositorio resulte caótico.

Los 3 comandos básicos para agregar nuestro proyecto a Githun, son:

~~~
git add .
git commit -m "Nombre de la nueva versión"
git push -u origin master
~~~
Pero, ¿qué significa "***add***" y ***commit***? ¿Por qué pasamos por estas dos fases?

!["Ejemplo"](https://cdn-images-1.medium.com/max/1600/0*HeEKExh4Z0nlev1m.png)

Ya habíamos visto anteriormente las fases de git, sino las recuerdas regresa a [GIT](https://github.com/PaulaSshun/tatooine/tree/master/SPRINT-2/01-GIT).

El código tiene 3 status en cada diferente fase, las más comunes son:
1. Modified
2. Staged
3. commited
