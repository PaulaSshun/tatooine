###### En el siguiente documento les mostraré algunos comandos y sus usos.

Local : Sólo se necesitan archivos y documentos locales para operar. Las lee directamente de tu base de datos local.

Remote : Mostrará los nombres de cada uno de los remotos que tienes especificados.

Init : Crea un nuevo repositorio de git.

Clone: Hace una copia desde su central del código a la computadora.

Add : Recibe la ruta de un archivo. Añade un nuevo archivo.

Commit : Identifica los cambios hechos en dicho ambiente de trabajo. Trabaja en tu repositorio local.

Push : Es un comando que sube los cambios hechos en tu ambiente de trabajo a una rama de trabajo tuya y/o de tu equipo remota. Trabaja a nivel de repositorio, es decir con tu repositorio remoto.

Pull : Es una abreviación de git fetch seguido de git merge FETCH_HEAD.
Baja los cambios de la rama determinada y la actualiza contra tu repositorio local.

Merge : Sirve para fucionar otra rama a tu rama activa.

#### FASES DE GIT
Para entender mejor git, se explica mejor dividiendolo por fases, las cuales serán presentadas a continuación:

1. Untracked: En esta fase no se lleva un regristro de ese archivo(s).

2. Tracked : Esos archivos ya se están registrando (cambios).

3. Modified: Ese archivo está siendo modificado.

4. Staged : Archivo que ya añadiste para hacer un snapshot o un commited. Es un registro de tiempo.

5. Commited: Archivo que ya se respaldó o se le hizo un snapshot en el tiempo.

#### COSAS QUE NO SE DEBEN HACER EN UN REPOSITORIO EN GIT

1. Nunca se debe de hacer commit directamente a 'master'.
Esto sobre todo aplica cuando trabajas colaborativamente usando un repositorio central principal pero también es válido si uno trabaja solo. Debemos evitar la mala costumbre de trabajar directamente sobre la rama master, no debemos trabajar nuestros cambios directamente pues estaremos perdiendo una de las características de Git, que es la capacidad de crear ramas instantáneamente (pues son solo la referencia a un commit).

2. Nunca subir archivos binarios.
Los datos acerca de cambios en archivos binarios hacen imposible leer los commits. Sin embargo, hay otra muy buena razón para dejar fuera de nuestro repositorio y es que, generalmente estos archivos como imágenes, binarios compilados o incluso videos son mucho más grandes que los archivos de texto de nuestro código y si hacemos commit de ellos a nuestro repositorio, el tamaño de este se volverá muy grande.

3. No usar fast forward.
No tenemos forma alguna de determinar en base a la historia la existencia de una rama y saber que commits fueron parte de esa feature.

#### ¿A que año debía volver Marty McFly para reestablecer la linea de tiempo?

El año al que tenía que volver era 1955.
